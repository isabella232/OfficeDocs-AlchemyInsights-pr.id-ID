---
title: Memindahkan pesan email ke kotak pesan arsip
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 41d6825b568263fb7b09066b65235aa348415bae
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/24/2019
ms.locfileid: "29474725"
---
<span data-ttu-id="d85dd-p101">Mengalami masalah pengarsipan item ke kotak pesan arsip. Pastikan Anda telah melakukan langkah-langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="d85dd-p101">Having problems archiving items to the Archive mailbox. Make sure you have performed the following steps:</span></span>
  
1. <span data-ttu-id="d85dd-p102">Mengkonfirmasi bahwa **arsip pesan** telah diaktifkan. Jika tidak, gunakan langkah-langkah dalam [artikel ini](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) untuk mengaktifkan kotak pesan arsip.</span><span class="sxs-lookup"><span data-stu-id="d85dd-p102">Confirm that an **Archive mailbox** has been enabled. If not, use steps in [this article](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span> 
    
2. <span data-ttu-id="d85dd-106">Di pusat Admin Exchange, pilih **Tag penyimpanan** di bawah **Manajemen kepatuhan**, membuat **tag penyimpanan** dengan tindakan **Pindahkan ke arsip** yang mengandung diinginkan **Waktu penyimpanan**.</span><span class="sxs-lookup"><span data-stu-id="d85dd-106">In the Exchange Admin Center, select **Retention Tags** under **Compliance Management**, create a **Retention tag** with the **Move to Archive** action containing the desired **Retention Age**.</span></span>
    
3. <span data-ttu-id="d85dd-107">Di pusat Admin Exchange, pilih **Kebijakan penyimpanan**, membuat **Kebijakan penyimpanan** dan menambahkan Anda **Pindahkan ke arsip** tag penyimpanan ke kebijakan itu.</span><span class="sxs-lookup"><span data-stu-id="d85dd-107">In the Exchange Admin Center, select **Retention Policies**, create a **Retention Policy** and add your **Move to Archive** retention tag to that policy.</span></span> 
    
4. <span data-ttu-id="d85dd-p103">[Menetapkan kebijakan penyimpanan](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) untuk kotak pesan pengguna tertentu. Kebijakan yang sama akan diterapkan ke **utama** dan kotak pesan **Arsip** .</span><span class="sxs-lookup"><span data-stu-id="d85dd-p103">[Assign the Retention Policy](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox. The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="d85dd-p104">Kotak pesan pengguna sekarang harus memiliki kebijakan pengarsipan untuk memindahkan item ke kotak pesan arsip. Mungkin perlu untuk memaksa berhasil Folder asisten (MFA) untuk menjalankan dan menerapkan pengaturan baru untuk kotak pesan pengguna. Jalankan perintah berikut saat [terhubung ke EXO PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) agar Bantuan Folder yang dikelola untuk kotak pesan tertentu:</span><span class="sxs-lookup"><span data-stu-id="d85dd-p104">The user's mailbox should now have an Archive policy to move items to the Archive mailbox. It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox. Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="d85dd-113">Ingin informasi lebih lanjut tentang pengaturan kebijakan pengarsipan, lihat [menetapkan kebijakan kotak pesan arsip dan penghapusan](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="d85dd-113">Want more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  

