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
ms.openlocfilehash: e2fb22f872be0eefc3b4b78b18cd09baffa66cda
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742436"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Kebijakan Penyimpanan di pusat admin Exchange

 **Terbitan:** Kebijakan retensi baru dibuat atau diperbarui di pusat admin Exchange tidak diterapkan ke kotak surat atau item tidak dipindahkan ke kotak surat Arsip atau dihapus. 
  
 **Akar penyebab:**
  
- Hal ini mungkin karena **bantuan folder yang dikelola** tidak memproses kotak surat pengguna. Bantuan folder yang dikelola mencoba memproses setiap kotak pesan di organisasi berbasis Internet setiap tujuh hari sekali. Jika Anda mengubah tag penyimpanan atau menerapkan kebijakan penyimpanan yang berbeda ke kotak pesan, Anda dapat menunggu hingga Bantuan Folder Terkelola memproses kotak pesan, atau Anda dapat menjalankan cmdlet Start-ManagedFolderAssistant untuk memulai bantuan folder yang dikelola untuk memproses kotak pesan tertentu. Menjalankan cmdlet ini berguna untuk pengujian atau pemecahan masalah pengaturan kebijakan penyimpanan atau tag penyimpanan. Untuk informasi lebih lanjut, kunjungi [menjalankan bantuan folder yang dikelola](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Solusi:** Jalankan perintah berikut ini untuk memulai bantuan folder yang dikelola untuk kotak pesan tertentu:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Hal ini juga dapat terjadi jika **Retentionhold** telah **diaktifkan** di kotak surat. Jika kotak surat telah ditempatkan di RetentionHold, kebijakan retensi di kotak surat tidak akan diproses selama waktu tersebut. Untuk informasi lebih lanjut tentang pengaturan RetentionHold Lihat: [kotak surat retensi tahan](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Solusi:**
    
  - Periksa status pengaturan RetentionHold pada kotak surat tertentu di [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Jalankan perintah berikut ini untuk **menonaktifkan** retentionhold di kotak surat tertentu:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Sekarang, jalankan kembali bantuan folder yang dikelola:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Catatan:** Jika kotak pesan lebih kecil dari 10 MB, Asisten folder yang dikelola tidak akan secara otomatis memproses kotak pesan.
 
Untuk informasi lebih lanjut tentang kebijakan retensi di pusat admin Exchange, lihat:
- [Tag penyimpanan dan kebijakan retensi](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Menerapkan kebijakan retensi ke kotak pesan](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Menambahkan atau menghapus tag penyimpanan](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Cara mengidentifikasi jenis terus ditempatkan di kotak surat](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
