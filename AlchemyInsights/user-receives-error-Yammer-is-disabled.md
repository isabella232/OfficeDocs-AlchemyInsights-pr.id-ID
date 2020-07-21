---
title: Pengguna menerima galat AADSTS7000112 Yammer dinonaktifkan
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198056"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a>Pengguna menerima galat AADSTS7000112 Yammer dinonaktifkan

Jika Anda menerima galat "AADSTS7000112: Application ' 00000005-0000-0ff1-ce00-000000000000 ' (heboh) dinonaktifkan", ada masalah dengan prinsipal layanan dalam Azure AD. Administrator mungkin telah dinonaktifkan prinsip layanan untuk memblokir akses ke Yammer.

Menonaktifkan pimpinan Layanan tidak disarankan dan dapat menyebabkan masalah tambahan. Untuk informasi lebih lanjut tentang pendekatan yang didukung untuk memblokir akses pengguna ke heboh, lihat [mematikan heboh akses untuk Microsoft 365 pengguna](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).  

Untuk memperbaiki masalah ini di Azure portal dan memulihkan akses pengguna ke Yammer:

1.  Buka halaman Azure Active Directory, dan pilih **aplikasi Enterprise** di bawah **Kelola** di panel navigasi kiri.
3.  Ketik **Office 365 heboh** di kotak pencarian, dan pilih nama aplikasi untuk membuka pengaturan.
4.  Pilih **properti** di bawah **Kelola** di panel navigasi kiri.
5.  Tetapkan nilai **diaktifkan bagi pengguna untuk masuk?** untuk **ya**, dan kemudian pilih **Simpan**.
6.  Masuk ke heboh lagi. Anda mungkin perlu menghapus cookie.

Selain itu, jalankan perintah PowerShell untuk menetapkan nilai. Untuk informasi lebih lanjut, lihat ["Maaf, tapi kami mengalami masalah saat masuk Anda" kesalahan ketika Anda mengklik ubin heboh di Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365). 