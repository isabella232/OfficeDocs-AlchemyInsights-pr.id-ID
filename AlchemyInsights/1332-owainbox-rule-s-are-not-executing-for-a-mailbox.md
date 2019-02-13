---
title: 1332 OWA - Inbox Bapepam tidak mengeksekusi untuk kotak pesan
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 0d3b7ce3d6b32d94a012eb3767c0747eed80f6e5
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/12/2019
ms.locfileid: "29915807"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="73d2a-102">Aturan kotak masuk tidak bekerja seperti yang diharapkan</span><span class="sxs-lookup"><span data-stu-id="73d2a-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="73d2a-103">Pastikan pengaturan berikut:</span><span class="sxs-lookup"><span data-stu-id="73d2a-103">Verify the following settings:</span></span>
  
- <span data-ttu-id="73d2a-p101">Pesan dapat diarahkan, diteruskan, atau menjawab secara otomatis berdasarkan aturan kotak masuk hanya satu kali. Aturan pengarah ulang (aturan kotak masuk atau pesan aliran aturan, juga dikenal sebagai aturan transport) dapat menambahkan maksimal sepuluh penerusan penerima pesan. Untuk selengkapnya, lihat [batas aturan jurnal, transportasi, dan kotak masuk](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="73d2a-p101">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time. A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message. For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>
    
- <span data-ttu-id="73d2a-p102">Aturan kotak masuk tidak bekerja pada kotak pesan alternatif Journal. Untuk selengkapnya tentang kotak pesan alternatif Journal, lihat [kotak pesan jurnal alternatif](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="73d2a-p102">Inbox rules don't work on the alternate journaling mailbox. For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>
    
<span data-ttu-id="73d2a-109">Untuk mengatasi masalah ini, lihat [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="73d2a-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>
  
<span data-ttu-id="73d2a-110">Jika masalah-masalah sebelumnya tidak berlaku, jalankan laporan diagnostik aturan kotak masuk sebelum Anda meneruskan masalah tersebut ke Microsoft Support:</span><span class="sxs-lookup"><span data-stu-id="73d2a-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>
  
1. <span data-ttu-id="73d2a-111">Membuka kotak pesan di Outlook di web, lalu klik **pengaturan** \> **pilihan** \> **mengatur email** \> **aturan kotak masuk**.</span><span class="sxs-lookup"><span data-stu-id="73d2a-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>
    
2. <span data-ttu-id="73d2a-112">Di bagian bawah laman, klik **jika aturan tidak bekerja klik di sini untuk menghasilkan laporan diagnostik**.</span><span class="sxs-lookup"><span data-stu-id="73d2a-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
    

