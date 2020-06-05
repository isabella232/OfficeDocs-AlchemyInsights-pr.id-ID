---
title: Pemecahan masalah acara dari email
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569139"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="46b91-102">Pemecahan masalah acara dari email</span><span class="sxs-lookup"><span data-stu-id="46b91-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="46b91-103">Verifikasi fitur diaktifkan untuk kotak surat: \*\*Get-EventsFromEmailConfiguration-identitas <mailbox> \*\*</span><span class="sxs-lookup"><span data-stu-id="46b91-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="46b91-104">Kemudian lihat di ' Events dari email ' log **ekspor-MailboxDiagnosticLogs <mailbox> -komponen timeprofile**</span><span class="sxs-lookup"><span data-stu-id="46b91-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="46b91-105">Di log "peristiwa dari email", Cari InternetMessageId yang cocok dengan item di kotak pesan.</span><span class="sxs-lookup"><span data-stu-id="46b91-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="46b91-106">Yang TrustScore menentukan apakah item yang ditambahkan atau tidak.</span><span class="sxs-lookup"><span data-stu-id="46b91-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="46b91-107">Acara hanya akan ditambahkan jika TrustScore = "Trusted".</span><span class="sxs-lookup"><span data-stu-id="46b91-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="46b91-108">TrustScore ditentukan oleh properti SPF, DKIM atau dMarc, yang berada di header pesan.</span><span class="sxs-lookup"><span data-stu-id="46b91-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="46b91-109">Untuk melihat properti ini:</span><span class="sxs-lookup"><span data-stu-id="46b91-109">To view these properties:</span></span>

<span data-ttu-id="46b91-110">**Desktop Outlook**</span><span class="sxs-lookup"><span data-stu-id="46b91-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="46b91-111">Membuka item</span><span class="sxs-lookup"><span data-stu-id="46b91-111">Open the item</span></span>
- <span data-ttu-id="46b91-112">Properti > file-header Internet ></span><span class="sxs-lookup"><span data-stu-id="46b91-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="46b91-113">Atau</span><span class="sxs-lookup"><span data-stu-id="46b91-113">or</span></span>

<span data-ttu-id="46b91-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="46b91-114">**MFCMapi**</span></span>

- <span data-ttu-id="46b91-115">Menavigasi ke item di kotak masuk</span><span class="sxs-lookup"><span data-stu-id="46b91-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="46b91-116">Cari PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="46b91-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="46b91-117">Properti ini ditentukan dan direkam selama transportasi dan perutean.</span><span class="sxs-lookup"><span data-stu-id="46b91-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="46b91-118">Untuk pemecahan masalah lebih lanjut, Anda mungkin perlu menindaklanjuti dengan dukungan transportasi tentang kegagalan dalam SPF, DKIM dan. atau DMARC.</span><span class="sxs-lookup"><span data-stu-id="46b91-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>