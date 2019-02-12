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
ms.openlocfilehash: a631af20e28a531a40f078e290239a372c38ab74
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/12/2019
ms.locfileid: "29941716"
---
Mengalami masalah pengarsipan item ke kotak pesan arsip. Pastikan Anda telah melakukan langkah-langkah berikut:
  
1. Mengkonfirmasi bahwa **arsip pesan** telah diaktifkan. Jika tidak, gunakan langkah-langkah dalam [artikel ini](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) untuk mengaktifkan kotak pesan arsip. 
    
2. Di pusat Admin Exchange, pilih **Tag penyimpanan** di bawah **Manajemen kepatuhan**, membuat **tag penyimpanan** dengan tindakan **Pindahkan ke arsip** yang mengandung diinginkan **Waktu penyimpanan**.
    
3. Di pusat Admin Exchange, pilih **Kebijakan penyimpanan**, membuat **Kebijakan penyimpanan** dan menambahkan Anda **Pindahkan ke arsip** tag penyimpanan ke kebijakan itu. 
    
4. [Menetapkan kebijakan penyimpanan](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) untuk kotak pesan pengguna tertentu. Kebijakan yang sama akan diterapkan ke **utama** dan kotak pesan **Arsip** . 
    
Kotak pesan pengguna sekarang harus memiliki kebijakan pengarsipan untuk memindahkan item ke kotak pesan arsip. Mungkin perlu untuk memaksa berhasil Folder asisten (MFA) untuk menjalankan dan menerapkan pengaturan baru untuk kotak pesan pengguna. Jalankan perintah berikut saat [terhubung ke EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) agar Bantuan Folder yang dikelola untuk kotak pesan tertentu: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

Ingin informasi lebih lanjut tentang pengaturan kebijakan pengarsipan, lihat [menetapkan kebijakan kotak pesan arsip dan penghapusan](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

