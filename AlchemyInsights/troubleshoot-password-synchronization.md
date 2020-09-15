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
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664929"
---
# <a name="troubleshoot-password-synchronization"></a>Memecahkan masalah sinkronisasi kata sandi

Untuk memecahkan masalah sinkronisasi kata sandi, mulai menggunakan tugas pemecahan masalah AAD ini untuk menentukan mengapa kata sandi tidak disinkronkan. Untuk memulai, masuk ke [Kelola sinkronisasi langsung](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Buka sesi Windows PowerShell baru di server Azure AD Connect Anda, lalu pilih opsi **Jalankan sebagai administrator** .

2. Jalankan set-ExecutionPolicy Remotesanye atau set-ExecutionPolicy tidak terbatas.

3. Mulai panduan Azure AD Connect.

4. Masuk ke halaman tugas tambahan > **memecahkan masalah**  >  **berikutnya**.

5. Pilih **Luncurkan** untuk membuka menu pemecahan masalah PowerShell.

6. Pilih **memecahkan masalah sinkronisasi kata sandi**.

    Masalah biasanya adalah kata sandi tidak disinkronkan untuk akun pengguna tertentu.

    **Catatan** Sinkronisasi kata sandi gagal jika sinkronisasi kata sandi yang terakhir berhasil adalah beberapa waktu yang lalu.

Untuk bantuan selengkapnya tentang pemecahan masalah sinkronisasi kata sandi, lihat [memecahkan masalah sinkronisasi hash kata sandi dengan sinkronisasi AZURE AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).