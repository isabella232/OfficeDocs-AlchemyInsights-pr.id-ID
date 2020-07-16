---
title: Tentang identitas di heboh
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148311"
---
# <a name="about-identity-in-yammer"></a>Tentang identitas di heboh

Sebaiknya semua jaringan mengambil langkah berikut untuk menghindari masalah terkait identitas:

1. Menegakkan Office 365 identitas setelah penyediaan Microsoft 365 akun untuk pengguna di Azure AD untuk memastikan bahwa semua pengguna masuk menggunakan akun Microsoft utama 365. Untuk informasi lebih lanjut, lihat [menegakkan Office 365 identitas pengguna heboh](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. Menggabungkan beberapa jaringan heboh. Legacy heboh konfigurasi mengizinkan beberapa heboh jaringan untuk dihubungkan ke satu penyewa. Untuk informasi lebih lanjut, lihat [jaringan migrasi-menggabungkan beberapa jaringan heboh](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. Opsional, menegakkan perizinan untuk heboh untuk memblokir pengguna dari heboh jika mereka tidak memiliki lisensi. Untuk informasi lebih lanjut, lihat [mengelola heboh pengguna lisensi di Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Akhirnya, audit daftar pengguna untuk jaringan heboh lama dan menangguhkan pengguna warisan. Disarankan agar Anda menangguhkan (menonaktifkan) pengguna, bukan menghapusnya, karena penghapusan ireversibel. Untuk informasi lebih lanjut, lihat [audit heboh pengguna di jaringan yang terhubung ke Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) dan [menghapus pengguna](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).

Dengan mengkonfigurasi heboh menggunakan langkah ini, Anda juga akan siap untuk mengkonfigurasi jaringan heboh Anda untuk mode asli untuk Microsoft 365. Untuk informasi lebih lanjut, lihat [mengkonfigurasi jaringan heboh Anda untuk mode asli untuk Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).