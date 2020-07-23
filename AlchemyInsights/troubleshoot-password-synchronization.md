---
title: Memecahkan masalah sinkronisasi sandi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387880"
---
# <a name="troubleshoot-password-synchronization"></a>Memecahkan masalah sinkronisasi sandi

Untuk memecahkan masalah sinkronisasi sandi, mulai menggunakan tugas pemecahan masalah AAD menghubungkan ini untuk menentukan mengapa sandi tidak menyinkronkan. Untuk memulai, buka [mengelola sinkronisasi langsung](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Buka sesi Windows PowerShell baru di server Azure AD menyambung, dan pilih opsi **Jalankan sebagai administrator** .

2. Jalankan set-ExecutionPolicy Remotesanye atau set-ExecutionPolicy terbatas.

3. Mulai Wisaya Azure AD menyambung.

4. Buka halaman tugas tambahan > **memecahkan masalah**  >  **berikutnya**.

5. Pilih **Luncurkan** untuk membuka menu pemecahan masalah PowerShell.

6. Pilih **memecahkan masalah sinkronisasi sandi**.

    Masalah ini biasanya bahwa sandi tidak disinkronkan untuk akun pengguna tertentu.

    **Notes** Sinkronisasi sandi gagal jika Sinkronisasi sandi berhasil terakhir adalah beberapa waktu yang lalu.

Untuk bantuan lebih lanjut pemecahan masalah sinkronisasi sandi, lihat [memecahkan masalah sinkronisasi hash sandi dengan AZURE AD menyambung sinkronisasi](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).