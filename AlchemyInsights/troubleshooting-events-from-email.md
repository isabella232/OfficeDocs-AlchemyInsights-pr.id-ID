---
title: Pemecahan Masalah Acara dari Email
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834842"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="03a4a-102">Pemecahan Masalah Acara dari Email</span><span class="sxs-lookup"><span data-stu-id="03a4a-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="03a4a-103">Memverifikasi bahwa fitur ini diaktifkan untuk kotak surat: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span><span class="sxs-lookup"><span data-stu-id="03a4a-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="03a4a-104">Lalu lihat log 'Acara dari Email' **Ekspor-Kotak SuratDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="03a4a-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="03a4a-105">Dalam log 'Acara dari Email', temukan InternetMessageId yang cocok dengan item dalam kotak surat.</span><span class="sxs-lookup"><span data-stu-id="03a4a-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="03a4a-106">TrustScore menentukan apakah item ditambahkan atau tidak.</span><span class="sxs-lookup"><span data-stu-id="03a4a-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="03a4a-107">Acara hanya akan ditambahkan jika TrustScore = "Trusted".</span><span class="sxs-lookup"><span data-stu-id="03a4a-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="03a4a-108">TrustScore ditentukan oleh properti SPF, Dkim atau Dmarc, yang ada di Header Pesan.</span><span class="sxs-lookup"><span data-stu-id="03a4a-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="03a4a-109">Untuk menampilkan properti ini:</span><span class="sxs-lookup"><span data-stu-id="03a4a-109">To view these properties:</span></span>

<span data-ttu-id="03a4a-110">**Desktop Outlook**</span><span class="sxs-lookup"><span data-stu-id="03a4a-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="03a4a-111">Membuka item</span><span class="sxs-lookup"><span data-stu-id="03a4a-111">Open the item</span></span>
- <span data-ttu-id="03a4a-112">File -> Properti -> Header Internet</span><span class="sxs-lookup"><span data-stu-id="03a4a-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="03a4a-113">atau</span><span class="sxs-lookup"><span data-stu-id="03a4a-113">or</span></span>

<span data-ttu-id="03a4a-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="03a4a-114">**MFCMapi**</span></span>

- <span data-ttu-id="03a4a-115">Menavigasi ke item dalam kotak masuk</span><span class="sxs-lookup"><span data-stu-id="03a4a-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="03a4a-116">Cari PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="03a4a-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="03a4a-117">Properti ini ditentukan dan direkam selama transportasi dan perutean.</span><span class="sxs-lookup"><span data-stu-id="03a4a-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="03a4a-118">Untuk pemecahan masalah lebih lanjut, Anda mungkin perlu menindaklanjuti Dukungan Transportasi tentang kegagalan di SPF, DKIM, dan.atau DMARC.</span><span class="sxs-lookup"><span data-stu-id="03a4a-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>