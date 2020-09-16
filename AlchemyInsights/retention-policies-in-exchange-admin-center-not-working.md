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
# <a name="retention-policies-in-exchange-admin-center"></a>Kebijakan Penyimpanan di pusat admin Exchange

Jika Anda ingin kami menjalankan pemeriksaan otomatis untuk pengaturan yang disebutkan di bawah ini, pilih tombol kembali <--di bagian atas Halaman ini, lalu masukkan alamat email pengguna yang mengalami masalah dengan kebijakan penyimpanan.

 **Masalah:** Kebijakan penyimpanan yang baru dibuat atau diperbarui di pusat admin Exchange tidak berlaku untuk kotak surat atau item tidak dipindahkan ke kotak surat Arsip atau dihapus. 
  
 **Akar penyebab:**
  
- Ini mungkin karena **bantuan folder yang dikelola** tidak memproses kotak surat pengguna. Bantuan folder yang dikelola mencoba memproses setiap kotak surat di organisasi berbasis awan Anda satu kali dalam tujuh hari. Jika Anda mengubah tag penyimpanan atau menerapkan kebijakan penyimpanan yang berbeda ke kotak surat, Anda bisa menunggu hingga folder yang dikelola membantu memproses kotak surat, atau Anda bisa menjalankan cmdlet Mulai-ManagedFolderAssistant untuk memulai bantuan folder yang dikelola untuk memproses kotak surat tertentu. Menjalankan cmdlet ini berguna untuk menguji atau memecahkan masalah pengaturan tag penyimpanan atau kebijakan penyimpanan. Untuk informasi selengkapnya, kunjungi [Jalankan asisten folder yang dikelola](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Solusi:** Jalankan perintah berikut ini untuk memulai bantuan folder yang dikelola untuk kotak surat tertentu:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Ini juga dapat terjadi jika **Retensionhold** telah **diaktifkan** pada kotak surat. Jika kotak surat telah ditempatkan pada penahanan ulang, kebijakan penyimpanan pada kotak surat tidak akan diproses selama waktu tersebut. Untuk informasi selengkapnya tentang pengaturan Retensionhold Lihat: penangguhan [penyimpanan kotak surat](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Solusi**
    
  - Periksa status pengaturan Retensionhold pada kotak surat tertentu di [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Jalankan perintah berikut ini untuk **menonaktifkan** retensionhold pada kotak surat tertentu:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Sekarang, jalankan kembali asisten folder yang dikelola:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Catatan:** Jika kotak surat lebih kecil dari 10 MB, Asisten folder yang dikelola tidak akan memproses kotak surat secara otomatis.
 
Untuk informasi selengkapnya tentang kebijakan penyimpanan di pusat admin Exchange, lihat:
- [Tag penyimpanan dan kebijakan penyimpanan](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Menerapkan kebijakan penyimpanan ke kotak surat](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Menambahkan atau menghapus tag penyimpanan](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Cara mengidentifikasi tipe penangguhan yang ditempatkan pada kotak surat](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
