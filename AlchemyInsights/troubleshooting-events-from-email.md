---
title: Pemecahan masalah acara dari email
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658737"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="2e137-102">Pemecahan masalah acara dari email</span><span class="sxs-lookup"><span data-stu-id="2e137-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="2e137-103">Verifikasi fitur diaktifkan untuk kotak surat: \*\*Get-EventsFromEmailConfiguration-identitas <mailbox> \*\*</span><span class="sxs-lookup"><span data-stu-id="2e137-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="2e137-104">Lalu lihat ' acara dari email ' log **Export-MailboxDiagnosticLogs <mailbox> -component timeprofile**</span><span class="sxs-lookup"><span data-stu-id="2e137-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="2e137-105">Dalam log ' acara dari email ', temukan InternetMessageId yang cocok dengan item dalam kotak surat.</span><span class="sxs-lookup"><span data-stu-id="2e137-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="2e137-106">Nilai Trustmenentukan Apakah item ditambahkan atau tidak.</span><span class="sxs-lookup"><span data-stu-id="2e137-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="2e137-107">Acara hanya akan ditambahkan jika TrustScore = "Trusted".</span><span class="sxs-lookup"><span data-stu-id="2e137-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="2e137-108">TrustScore ditentukan oleh SPF, DKIM atau properti dMarc, yang berada di header pesan.</span><span class="sxs-lookup"><span data-stu-id="2e137-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="2e137-109">Untuk menampilkan properti ini:</span><span class="sxs-lookup"><span data-stu-id="2e137-109">To view these properties:</span></span>

<span data-ttu-id="2e137-110">**Outlook desktop**</span><span class="sxs-lookup"><span data-stu-id="2e137-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="2e137-111">Membuka item</span><span class="sxs-lookup"><span data-stu-id="2e137-111">Open the item</span></span>
- <span data-ttu-id="2e137-112">Properti file->-header Internet ></span><span class="sxs-lookup"><span data-stu-id="2e137-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="2e137-113">atau</span><span class="sxs-lookup"><span data-stu-id="2e137-113">or</span></span>

<span data-ttu-id="2e137-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="2e137-114">**MFCMapi**</span></span>

- <span data-ttu-id="2e137-115">Menavigasi ke item dalam kotak masuk</span><span class="sxs-lookup"><span data-stu-id="2e137-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="2e137-116">Cari PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="2e137-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="2e137-117">Properti ini ditentukan dan direkam selama pengangkutan dan perutean.</span><span class="sxs-lookup"><span data-stu-id="2e137-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="2e137-118">Untuk pemecahan masalah lebih lanjut, Anda mungkin perlu menindaklanjuti dukungan transportasi tentang kegagalan SPF, DKIM, dan. or DMARC.</span><span class="sxs-lookup"><span data-stu-id="2e137-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>