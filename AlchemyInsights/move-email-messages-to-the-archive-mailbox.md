---
title: Memindahkan pesan email ke kotak surat Arsip
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
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 7e72766f441e210a81fcfd6c07b1801f6c0474afb02a70edf2ad8dbb571f3d2a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974960"
---
# <a name="move-email-to-the-archive-mailbox"></a>Memindahkan email ke kotak surat arsip

Jika Anda ingin kami menjalankan pemeriksaan otomatis untuk pengaturan yang disebutkan di bawah ini, pilih tombol kembali <-- di bagian atas halaman ini, lalu masukkan alamat email pengguna yang mengalami masalah dalam memindahkan email ke kotak surat arsip mereka.

1. Konfirmasi bahwa **kotak surat Arsip** telah diaktifkan. Jika tidak, gunakan langkah-langkah [dalam artikel ini](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) untuk mengaktifkan kotak surat arsip.

2. Untuk mengarsipkan pesan secara otomatis ke kotak  surat arsip, tag penyimpanan dengan tindakan Pindahkan ke arsip harus diatur agar diterapkan secara otomatis ke **seluruh tag kotak surat (default).** Gunakan langkah-langkah di sini untuk membuat tag: [Tag Arsip Default.](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag)

3. Berikutnya, tambahkan tag **Arsip** ke kebijakan penyimpanan Anda. Di pusat admin Exchange, **pilih** Kebijakan Penyimpanan > menambahkan **tag** Pindahkan ke Arsip ke > **simpan.**

4. Sekarang [Tetapkan Kebijakan Penyimpanan](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) ke kotak surat pengguna tertentu. Kebijakan yang sama akan diterapkan ke kotak **surat** Utama **dan** Arsip.

Anda mungkin perlu memaksa Asisten Folder Terkelola (MFA, Managed Folder Assistant) untuk menjalankan dan menerapkan pengaturan baru ke kotak surat pengguna. Jalankan perintah berikut ketika [terhubung ke PowerShell EXO untuk](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) memulai Asisten Folder Terkelola untuk kotak surat tertentu:
  
Start-ManagedFolderAssistant -Identity <name of the mailbox>

Untuk informasi selengkapnya tentang menyiapkan kebijakan arsip, lihat [Menyiapkan kebijakan arsip dan penghapusan untuk kotak surat](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  