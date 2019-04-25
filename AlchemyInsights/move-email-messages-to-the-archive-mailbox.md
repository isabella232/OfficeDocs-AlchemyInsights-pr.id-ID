---
title: Memindahkan pesan email ke kotak pesan arsip
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 37f256ef31402f5139fdd7c2af8f3a6ca9dc3525
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/23/2019
ms.locfileid: "32418318"
---
# <a name="move-email-to-the-archive-mailbox"></a>Memindahkan email ke kotak pesan arsip
 
1. Mengkonfirmasi bahwa **arsip pesan** telah diaktifkan. Jika tidak, gunakan langkah-langkah dalam [artikel ini](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) untuk mengaktifkan kotak pesan arsip.

2. Arsip pesan otomatis ke kotak pesan arsip, tag penyimpanan dengan tindakan **Pindahkan ke arsip** harus ditetapkan **secara otomatis**diterapkan tag seluruh kotak (default). Gunakan langkah-langkah berikut untuk membuat tag: [tag arsip Default](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).
    
3. Selanjutnya, Tambahkan tag **Arsip** ke kebijakan penyimpanan Anda. Di pusat admin Exchange, pilih **Kebijakan penyimpanan** > menambahkan **Pindahkan ke arsip tag** ke > kebijakan yang **menyelamatkan**. 
    
4. Sekarang [menetapkan kebijakan penyimpanan](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) untuk kotak pesan pengguna tertentu. Kebijakan yang sama akan diterapkan ke **utama** dan kotak pesan **Arsip** . 
    
Mungkin perlu untuk memaksa berhasil Folder asisten (MFA) untuk menjalankan dan menerapkan pengaturan baru untuk kotak pesan pengguna. Jalankan perintah berikut saat [terhubung ke EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) agar Bantuan Folder yang dikelola untuk kotak pesan tertentu: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

Untuk informasi lebih lanjut tentang pengaturan kebijakan pengarsipan, lihat [menetapkan kebijakan kotak pesan arsip dan penghapusan](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

