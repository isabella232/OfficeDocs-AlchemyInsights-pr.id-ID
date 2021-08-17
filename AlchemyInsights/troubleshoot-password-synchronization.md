---
title: Memecahkan masalah sinkronisasi kata sandi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: cb782c0d1dc396ee7a9f016afb9629a2cdee93d52f5408b7a73e576e783ebc0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105755"
---
# <a name="troubleshoot-password-synchronization"></a>Memecahkan masalah sinkronisasi kata sandi

Untuk memecahkan masalah sinkronisasi kata sandi, mulailah dengan menggunakan AAD Koneksi memecahkan masalah untuk menentukan mengapa kata sandi tidak tersinkron. Untuk memulai, buka [Mengelola sinkronisasi langsung](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Buka sesi Windows PowerShell baru di server Azure AD Koneksi, lalu pilih **opsi Jalankan sebagai** Administrator.

2. Jalankan Set-ExecutionPolicy RemoteSigned atau Set-ExecutionPolicy Tidak Terbatas.

3. Mulai panduan Koneksi Azure AD.

4. Masuk ke halaman Tugas Tambahan > **Pemecahan**  >  **Masalah Berikutnya.**

5. Pilih **Luncurkan** untuk membuka menu pemecahan masalah PowerShell.

6. Pilih **Pecahkan Masalah Sinkronisasi Kata Sandi.**

    Masalah biasanya adalah kata sandi tidak disinkronkan untuk akun pengguna tertentu.

    **Catatan** Sinkronisasi kata sandi gagal jika sinkronisasi kata sandi yang berhasil terakhir dilakukan beberapa waktu lalu.

Untuk bantuan selengkapnya dalam memecahkan masalah sinkronisasi kata sandi, [lihat Memecahkan masalah sinkronisasi hash kata sandi dengan Azure AD Koneksi sinkronisasi](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).