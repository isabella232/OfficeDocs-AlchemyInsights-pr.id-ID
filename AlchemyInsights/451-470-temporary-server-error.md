---
title: 451 4.7.0 Kesalahan server sementara. Silakan coba lagi nanti. PRX4
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2021
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "3000003"
- "12465"
ms.openlocfilehash: ce898981d053c8b5dc080ee83434bdacd7f02a636f0183293915bacdb48ba4ef
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812582"
---
# <a name="451-470-temporary-server-error-please-try-again-later-prx4"></a>451 4.7.0 Kesalahan server sementara. Silakan coba lagi nanti. PRX4

Anda mungkin mengalami masalah saat mengirimkan email melalui Smarthost "smtp.office365.com" menggunakan metode Pengiriman Klien SMTP dan menerima kesalahan: "Kesalahan server sementara 451 4.7.0. Silakan coba lagi nanti. PRX4 sebagian besar bersifat sementara." 

Pastikan Anda tidak menggunakan kotak surat bersama untuk Pengiriman Klien SMTP, karena metode Pengiriman klien SMTP memerlukan kotak surat berlisensi untuk mengirim email. Namun, jika Anda tidak menggunakan kotak surat bersama dan masalah tetap terjadi, periksa hal berikut:

1. Aktifkan pengiriman SMTP Klien pada kotak surat berlisensi yang sedang digunakan dengan menjalankan perintah PowerShell ini:

    ```Set-CASMailbox -Identity sean@contoso.com -SmtpClientAuthenticationDisabled $false```

    ATAU

    1. Masuk ke pusat admin Microsoft 365 > **Pengguna aktif**, dan pilih pengguna.
    1. Masuk ke tab Email > **Aplikasi email** > pilih Kelola **aplikasi email**. 
    1. Pastikan pengaturan **SMTP Terautentikasi** dicentang (diaktifkan).
    1. Pilih **Simpan perubahan.**
    
    Untuk mengaktifkan Autentikasi SMTP untuk seluruh organisasi, jalankan perintah ini:

    `Set-TransportConfig -SmtpClientAuthenticationDisabled $true`
 
    **Catatan**: Untuk alasan keamanan, sebaiknya aktifkan Autentikasi SMTP hanya agar kotak surat digunakan. Pengaturan tingkat pengguna menimpa pengaturan tingkat organisasi.

2. Nonaktifkan Default Keamanan Azure dengan mengaktifkan **keamanan default ke** **Tidak:**

    1. Masuk ke portal Azure sebagai administrator keamanan, administrator Akses Kondisional, atau administrator global.
    1. Telusuri ke Azure Active Directory >**  Properti**, dan **pilih Kelola keamanan default.**
    1. Atur tombol **aktifkan default keamanan** menjadi **Tidak**.
    1. Pilih **Simpan**.

3. Menonaktifkan Multi Factor Authentication (MFA) pada kotak surat berlisensi yang digunakan.

    1. Masuk ke pusat admin Microsoft 365, dan di menu navigasi kiri pilih **Pengguna**  >  **Aktif pengguna.**
    1. Di halaman **Pengguna aktif,** pilih **Autentikasi multi-faktor**.
    1. Pilih pengguna dan nonaktifkan **Autentikasi multiftor.**

