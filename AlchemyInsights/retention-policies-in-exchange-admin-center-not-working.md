---
title: Kebijakan Penyimpanan di Exchange Admin Center tidak bekerja
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 5d7b62546397c13b37540e8797b31123b2880280
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551346"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="5511e-102">Kebijakan Penyimpanan di Exchange Admin Center</span><span class="sxs-lookup"><span data-stu-id="5511e-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="5511e-103">**Masalah:** Baru dibuat atau kebijakan penyimpanan yang diperbarui di pusat Admin asing tidak berlaku untuk kotak pesan atau item tidak dipindahkan ke kotak pesan arsip atau dihapus.</span><span class="sxs-lookup"><span data-stu-id="5511e-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="5511e-104">**Akar penyebab:**</span><span class="sxs-lookup"><span data-stu-id="5511e-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="5511e-105">Ini mungkin karena **Bantuan Folder yang dikelola** tidak diproses kotak pesan pengguna.</span><span class="sxs-lookup"><span data-stu-id="5511e-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="5511e-106">Bantuan Folder yang dikelola akan mencoba memproses setiap kotak pesan di organisasi berbasis Internet setiap tujuh hari sekali.</span><span class="sxs-lookup"><span data-stu-id="5511e-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="5511e-107">Jika Anda mengubah tag penyimpanan atau menerapkan kebijakan penyimpanan yang berbeda ke kotak pesan, Anda dapat menunggu sampai membantu Folder dikelola memproses kotak pesan, atau Anda dapat menjalankan cmdlet Mulai-ManagedFolderAssistant untuk memulai Bantuan Folder yang dikelola untuk memproses tertentu kotak pesan.</span><span class="sxs-lookup"><span data-stu-id="5511e-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="5511e-108">Menjalankan cmdlet ini berguna untuk menguji atau mengatasi masalah kebijakan penyimpanan atau pengaturan tag penyimpanan.</span><span class="sxs-lookup"><span data-stu-id="5511e-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="5511e-109">Untuk informasi lebih lanjut, kunjungi [menjalankan Bantuan Folder yang dikelola](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="5511e-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="5511e-110">**Solusi:** Jalankan perintah berikut agar Bantuan Folder yang dikelola untuk kotak pesan tertentu:</span><span class="sxs-lookup"><span data-stu-id="5511e-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="5511e-111">Ini dapat juga dapat terjadi jika **penahanan penyimpanan** telah **diaktifkan** pada kotak pesan.</span><span class="sxs-lookup"><span data-stu-id="5511e-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="5511e-112">Jika kotak pesan yang telah ditempatkan di penahanan penyimpanan, kebijakan penyimpanan pada kotak pesan tidak akan diproses selama waktu itu.</span><span class="sxs-lookup"><span data-stu-id="5511e-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="5511e-113">Untuk lebih banyak informasi di lihat pengaturan penahanan penyimpanan: [Kotak penyimpanan terus](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="5511e-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="5511e-114">**Solusi:**</span><span class="sxs-lookup"><span data-stu-id="5511e-114">**Solution:**</span></span>
    
  - <span data-ttu-id="5511e-115">Memeriksa status pengaturan penahanan penyimpanan pada kotak pesan tertentu di [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="5511e-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="5511e-116">Jalankan perintah berikut agar dapat **menonaktifkan** penahanan penyimpanan pada kotak pesan tertentu:</span><span class="sxs-lookup"><span data-stu-id="5511e-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="5511e-117">Sekarang, kembali menjalankan folder Managed asisten:</span><span class="sxs-lookup"><span data-stu-id="5511e-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="5511e-118">**Catatan:** Jika kotak pesan yang lebih kecil dari 10 MB, Bantuan Folder yang dikelola tidak akan secara otomatis memproses kotak pesan.</span><span class="sxs-lookup"><span data-stu-id="5511e-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="5511e-119">Untuk info lebih lanjut tentang kebijakan penyimpanan di Exchange Admin Center, lihat:</span><span class="sxs-lookup"><span data-stu-id="5511e-119">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="5511e-120">Kebijakan Penyimpanan dan tag penyimpanan</span><span class="sxs-lookup"><span data-stu-id="5511e-120">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="5511e-121">Menerapkan kebijakan penyimpanan ke kotak pesan</span><span class="sxs-lookup"><span data-stu-id="5511e-121">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="5511e-122">Menambah atau menghapus tag penyimpanan</span><span class="sxs-lookup"><span data-stu-id="5511e-122">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="5511e-123">Bagaimana mengidentifikasi jenis memegang ditempatkan pada kotak pesan</span><span class="sxs-lookup"><span data-stu-id="5511e-123">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
