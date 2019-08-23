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
# <a name="retention-policies-in-exchange-admin-center"></a>Kebijakan Penyimpanan di Exchange Admin Center

 **Masalah:** Baru dibuat atau kebijakan penyimpanan yang diperbarui di pusat Admin asing tidak berlaku untuk kotak pesan atau item tidak dipindahkan ke kotak pesan arsip atau dihapus. 
  
 **Akar penyebab:**
  
- Ini mungkin karena **Bantuan Folder yang dikelola** tidak diproses kotak pesan pengguna. Bantuan Folder yang dikelola akan mencoba memproses setiap kotak pesan di organisasi berbasis Internet setiap tujuh hari sekali. Jika Anda mengubah tag penyimpanan atau menerapkan kebijakan penyimpanan yang berbeda ke kotak pesan, Anda dapat menunggu sampai membantu Folder dikelola memproses kotak pesan, atau Anda dapat menjalankan cmdlet Mulai-ManagedFolderAssistant untuk memulai Bantuan Folder yang dikelola untuk memproses tertentu kotak pesan. Menjalankan cmdlet ini berguna untuk menguji atau mengatasi masalah kebijakan penyimpanan atau pengaturan tag penyimpanan. Untuk informasi lebih lanjut, kunjungi [menjalankan Bantuan Folder yang dikelola](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Solusi:** Jalankan perintah berikut agar Bantuan Folder yang dikelola untuk kotak pesan tertentu:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Ini dapat juga dapat terjadi jika **penahanan penyimpanan** telah **diaktifkan** pada kotak pesan. Jika kotak pesan yang telah ditempatkan di penahanan penyimpanan, kebijakan penyimpanan pada kotak pesan tidak akan diproses selama waktu itu. Untuk lebih banyak informasi di lihat pengaturan penahanan penyimpanan: [Kotak penyimpanan terus](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Solusi:**
    
  - Memeriksa status pengaturan penahanan penyimpanan pada kotak pesan tertentu di [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
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
 
Untuk info lebih lanjut tentang kebijakan penyimpanan di Exchange Admin Center, lihat:
- [Kebijakan Penyimpanan dan tag penyimpanan](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Menerapkan kebijakan penyimpanan ke kotak pesan](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Menambah atau menghapus tag penyimpanan](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Bagaimana mengidentifikasi jenis memegang ditempatkan pada kotak pesan](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
