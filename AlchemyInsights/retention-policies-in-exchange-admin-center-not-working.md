---
title: Kebijakan Penyimpanan di Exchange Admin Center tidak bekerja
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 0ceb1737040f0304bfe8b611241ce1deef487652
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/24/2019
ms.locfileid: "29474979"
---
 **Masalah:** Baru dibuat atau kebijakan penyimpanan yang diperbarui di pusat Admin asing tidak berlaku untuk kotak pesan atau item tidak dipindahkan ke kotak pesan arsip atau dihapus. 
  
 **Akar penyebab:**
  
- Ini mungkin karena **Bantuan Folder yang dikelola** tidak diproses kotak pesan pengguna. Bantuan Folder yang dikelola akan mencoba memproses setiap kotak pesan di organisasi berbasis Internet setiap tujuh hari sekali. Jika Anda mengubah tag penyimpanan atau menerapkan kebijakan penyimpanan yang berbeda ke kotak pesan, Anda dapat menunggu sampai membantu Folder dikelola memproses kotak pesan, atau Anda dapat menjalankan cmdlet Mulai-ManagedFolderAssistant untuk memulai Bantuan Folder yang dikelola untuk memproses tertentu kotak pesan. Menjalankan cmdlet ini berguna untuk menguji atau mengatasi masalah kebijakan penyimpanan atau pengaturan tag penyimpanan. Untuk informasi lebih lanjut, kunjungi [menjalankan Bantuan Folder yang dikelola](https://msdn.microsoft.com/en-us/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Solusi:** Jalankan perintah berikut agar Bantuan Folder yang dikelola untuk kotak pesan tertentu: 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Ini dapat juga dapat terjadi jika **penahanan penyimpanan** telah **diaktifkan** pada kotak pesan. Jika kotak pesan yang telah ditempatkan di penahanan penyimpanan, kebijakan penyimpanan pada kotak pesan tidak akan diproses selama waktu itu. Untuk lebih banyak informasi di lihat pengaturan penahanan penyimpanan: [Kotak penyimpanan terus](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    Solusi
    
  - Memeriksa status pengaturan penahanan penyimpanan pada kotak pesan tertentu di [EXO powershell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Jalankan perintah berikut agar dapat **menonaktifkan** penahanan penyimpanan pada kotak pesan tertentu: 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Sekarang, kembali menjalankan folder Managed asisten:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Catatan:** Jika kotak pesan yang lebih kecil dari 10 MB, Bantuan Folder yang dikelola tidak akan secara otomatis memproses kotak pesan. 
  

