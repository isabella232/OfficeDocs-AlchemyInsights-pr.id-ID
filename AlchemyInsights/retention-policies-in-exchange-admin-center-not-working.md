---
title: Kebijakan Penyimpanan di pusat admin Exchange tidak berfungsi
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740513"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="d66fc-102">Kebijakan Penyimpanan di pusat admin Exchange</span><span class="sxs-lookup"><span data-stu-id="d66fc-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="d66fc-103">Jika Anda ingin kami menjalankan pemeriksaan otomatis untuk pengaturan yang disebutkan di bawah ini, pilih tombol kembali <--di bagian atas Halaman ini, lalu masukkan alamat email pengguna yang mengalami masalah dengan kebijakan penyimpanan.</span><span class="sxs-lookup"><span data-stu-id="d66fc-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="d66fc-104">**Masalah:** Kebijakan penyimpanan yang baru dibuat atau diperbarui di pusat admin Exchange tidak berlaku untuk kotak surat atau item tidak dipindahkan ke kotak surat Arsip atau dihapus.</span><span class="sxs-lookup"><span data-stu-id="d66fc-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="d66fc-105">**Akar penyebab:**</span><span class="sxs-lookup"><span data-stu-id="d66fc-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="d66fc-106">Ini mungkin karena **bantuan folder yang dikelola** tidak memproses kotak surat pengguna.</span><span class="sxs-lookup"><span data-stu-id="d66fc-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="d66fc-107">Bantuan folder yang dikelola mencoba memproses setiap kotak surat di organisasi berbasis awan Anda satu kali dalam tujuh hari.</span><span class="sxs-lookup"><span data-stu-id="d66fc-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="d66fc-108">Jika Anda mengubah tag penyimpanan atau menerapkan kebijakan penyimpanan yang berbeda ke kotak surat, Anda bisa menunggu hingga folder yang dikelola membantu memproses kotak surat, atau Anda bisa menjalankan cmdlet Mulai-ManagedFolderAssistant untuk memulai bantuan folder yang dikelola untuk memproses kotak surat tertentu.</span><span class="sxs-lookup"><span data-stu-id="d66fc-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="d66fc-109">Menjalankan cmdlet ini berguna untuk menguji atau memecahkan masalah pengaturan tag penyimpanan atau kebijakan penyimpanan.</span><span class="sxs-lookup"><span data-stu-id="d66fc-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="d66fc-110">Untuk informasi selengkapnya, kunjungi [Jalankan asisten folder yang dikelola](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="d66fc-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="d66fc-111">**Solusi:** Jalankan perintah berikut ini untuk memulai bantuan folder yang dikelola untuk kotak surat tertentu:</span><span class="sxs-lookup"><span data-stu-id="d66fc-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="d66fc-112">Ini juga dapat terjadi jika **Retensionhold** telah **diaktifkan** pada kotak surat.</span><span class="sxs-lookup"><span data-stu-id="d66fc-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="d66fc-113">Jika kotak surat telah ditempatkan pada penahanan ulang, kebijakan penyimpanan pada kotak surat tidak akan diproses selama waktu tersebut.</span><span class="sxs-lookup"><span data-stu-id="d66fc-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="d66fc-114">Untuk informasi selengkapnya tentang pengaturan Retensionhold Lihat: penangguhan [penyimpanan kotak surat](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="d66fc-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="d66fc-115">**Solusi**</span><span class="sxs-lookup"><span data-stu-id="d66fc-115">**Solution:**</span></span>
    
  - <span data-ttu-id="d66fc-116">Periksa status pengaturan Retensionhold pada kotak surat tertentu di [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="d66fc-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="d66fc-117">Jalankan perintah berikut ini untuk **menonaktifkan** retensionhold pada kotak surat tertentu:</span><span class="sxs-lookup"><span data-stu-id="d66fc-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="d66fc-118">Sekarang, jalankan kembali asisten folder yang dikelola:</span><span class="sxs-lookup"><span data-stu-id="d66fc-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="d66fc-119">**Catatan:** Jika kotak surat lebih kecil dari 10 MB, Asisten folder yang dikelola tidak akan memproses kotak surat secara otomatis.</span><span class="sxs-lookup"><span data-stu-id="d66fc-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="d66fc-120">Untuk informasi selengkapnya tentang kebijakan penyimpanan di pusat admin Exchange, lihat:</span><span class="sxs-lookup"><span data-stu-id="d66fc-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="d66fc-121">Tag penyimpanan dan kebijakan penyimpanan</span><span class="sxs-lookup"><span data-stu-id="d66fc-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="d66fc-122">Menerapkan kebijakan penyimpanan ke kotak surat</span><span class="sxs-lookup"><span data-stu-id="d66fc-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="d66fc-123">Menambahkan atau menghapus tag penyimpanan</span><span class="sxs-lookup"><span data-stu-id="d66fc-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="d66fc-124">Cara mengidentifikasi tipe penangguhan yang ditempatkan pada kotak surat</span><span class="sxs-lookup"><span data-stu-id="d66fc-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
