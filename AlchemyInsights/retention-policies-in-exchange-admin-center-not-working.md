---
title: Kebijakan Penyimpanan di pusat admin Exchange tidak berfungsi
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 4d3ca121c8d22a0900f136f7f2a754dfb5b435f5
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522810"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="f3e03-102">Kebijakan Penyimpanan di pusat admin Exchange</span><span class="sxs-lookup"><span data-stu-id="f3e03-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="f3e03-103">Jika Anda ingin kami menjalankan pemeriksaan otomatis untuk pengaturan yang disebutkan di bawah, pilih tombol kembali <--di bagian atas Halaman ini, lalu masukkan alamat email pengguna yang memiliki masalah dengan kebijakan retensi.</span><span class="sxs-lookup"><span data-stu-id="f3e03-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="f3e03-104">**Terbitan:** Kebijakan retensi baru dibuat atau diperbarui di pusat admin Exchange tidak diterapkan ke kotak surat atau item tidak dipindahkan ke kotak surat Arsip atau dihapus.</span><span class="sxs-lookup"><span data-stu-id="f3e03-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="f3e03-105">**Akar penyebab:**</span><span class="sxs-lookup"><span data-stu-id="f3e03-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="f3e03-106">Hal ini mungkin karena **bantuan folder yang dikelola** tidak memproses kotak surat pengguna.</span><span class="sxs-lookup"><span data-stu-id="f3e03-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="f3e03-107">Bantuan folder yang dikelola mencoba memproses setiap kotak pesan di organisasi berbasis Internet setiap tujuh hari sekali.</span><span class="sxs-lookup"><span data-stu-id="f3e03-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="f3e03-108">Jika Anda mengubah tag penyimpanan atau menerapkan kebijakan penyimpanan yang berbeda ke kotak pesan, Anda dapat menunggu hingga Bantuan Folder Terkelola memproses kotak pesan, atau Anda dapat menjalankan cmdlet Start-ManagedFolderAssistant untuk memulai bantuan folder yang dikelola untuk memproses kotak pesan tertentu.</span><span class="sxs-lookup"><span data-stu-id="f3e03-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="f3e03-109">Menjalankan cmdlet ini berguna untuk pengujian atau pemecahan masalah pengaturan kebijakan penyimpanan atau tag penyimpanan.</span><span class="sxs-lookup"><span data-stu-id="f3e03-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="f3e03-110">Untuk informasi lebih lanjut, kunjungi [menjalankan bantuan folder yang dikelola](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="f3e03-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="f3e03-111">**Solusi:** Jalankan perintah berikut ini untuk memulai bantuan folder yang dikelola untuk kotak pesan tertentu:</span><span class="sxs-lookup"><span data-stu-id="f3e03-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="f3e03-112">Hal ini juga dapat terjadi jika **Retentionhold** telah **diaktifkan** di kotak surat.</span><span class="sxs-lookup"><span data-stu-id="f3e03-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="f3e03-113">Jika kotak surat telah ditempatkan di RetentionHold, kebijakan retensi di kotak surat tidak akan diproses selama waktu tersebut.</span><span class="sxs-lookup"><span data-stu-id="f3e03-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="f3e03-114">Untuk informasi lebih lanjut tentang pengaturan RetentionHold Lihat: [kotak surat retensi tahan](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="f3e03-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="f3e03-115">**Solusi:**</span><span class="sxs-lookup"><span data-stu-id="f3e03-115">**Solution:**</span></span>
    
  - <span data-ttu-id="f3e03-116">Periksa status pengaturan RetentionHold pada kotak surat tertentu di [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="f3e03-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="f3e03-117">Jalankan perintah berikut ini untuk **menonaktifkan** retentionhold di kotak surat tertentu:</span><span class="sxs-lookup"><span data-stu-id="f3e03-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="f3e03-118">Sekarang, jalankan kembali bantuan folder yang dikelola:</span><span class="sxs-lookup"><span data-stu-id="f3e03-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="f3e03-119">**Catatan:** Jika kotak pesan lebih kecil dari 10 MB, Asisten folder yang dikelola tidak akan secara otomatis memproses kotak pesan.</span><span class="sxs-lookup"><span data-stu-id="f3e03-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="f3e03-120">Untuk informasi lebih lanjut tentang kebijakan retensi di pusat admin Exchange, lihat:</span><span class="sxs-lookup"><span data-stu-id="f3e03-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="f3e03-121">Tag penyimpanan dan kebijakan retensi</span><span class="sxs-lookup"><span data-stu-id="f3e03-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="f3e03-122">Menerapkan kebijakan retensi ke kotak pesan</span><span class="sxs-lookup"><span data-stu-id="f3e03-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="f3e03-123">Menambahkan atau menghapus tag penyimpanan</span><span class="sxs-lookup"><span data-stu-id="f3e03-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="f3e03-124">Cara mengidentifikasi jenis terus ditempatkan di kotak surat</span><span class="sxs-lookup"><span data-stu-id="f3e03-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
