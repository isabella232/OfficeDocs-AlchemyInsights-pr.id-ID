---
title: Contoh Pertahanan Microsoft untuk Office 365 kebijakan anti-phishing
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: b59abdeea6ac9be7e498e2b1ba531e7bf611c92097fbc12237e78364dae84f35
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54035009"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Contoh Pertahanan Microsoft untuk Office 365 kebijakan anti-phishing

Pengaturan ini mengaktifkan kebijakan yang disebut *Domain dan CEO*. Kebijakan ini menyediakan baik pengguna dan proteksi domain dari penyamaran lalu menerapkan kebijakan untuk semua email yang diterima oleh pengguna di dalam domain. Pertama, tambahkan informasi berikut ini untuk membuat kebijakan:

- **Nama**: Deskripsi Domain **dan CEO**: Memastikan bahwa CEO dan domain Anda tidak diirukan.
  **Diterapkan ke**: **Pilih Domain penerima adalah**. Di **bawah Salah satu** dari ini , **pilih** Pilih , lalu pilih domain. Pilih **+ Tambah.** Pilih kotak centang di samping nama domain dalam daftar (misalnya, klik *contoso.com*), lalu pilih **Tambahkan**. Pilih **Selesai.**
- Setelah kebijakan dibuat, Anda dapat menyelaraskan kebijakan dengan menggunakan opsi berikut:
  - **Tambahkan pengguna untuk melindungi:** Untuk contoh ini, tambahkan alamat email CEO, minimal.
  - **Tambahkan domain untuk diproteksi:** Tambahkan domain organisasi yang menyertakan kantor CEO.
  - **Memilih tindakan**: **Untuk jika email** dikirim oleh pengguna yang meniru , pilih Alihkan pesan ke alamat email lain , lalu masukkan alamat **email** administrator keamanan (misalnya, *securityadmin@contoso.com*). Untuk **Jika email dikirim oleh domain yang meniru**, pilih **Karantina pesan**.
  - **Kecerdasan kotak** surat : Secara default, opsi ini dipilih saat Anda membuat kebijakan anti-phishing baru. Biarkan pengaturan ini **Di Tempat** untuk mendapatkan hasil terbaik.
  - **Menambahkan pengirim dan domain tepercaya:** Untuk contoh ini, jangan mendefinisikan penggantian apa pun.
- Setelah Anda meninjau pengaturan Anda, pilih Buat **kebijakan ini atau Simpan** , sebagaimana diperlukan. 

Untuk mempelajari selengkapnya, lihat [Kebijakan anti-phishing Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).
