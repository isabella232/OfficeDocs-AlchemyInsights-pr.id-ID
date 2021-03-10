---
title: Contoh Microsoft Defender untuk kebijakan anti-phishing Office 365
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
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694035"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Contoh Microsoft Defender untuk kebijakan anti-phishing Office 365

Pengaturan ini mengaktifkan kebijakan yang disebut *domain dan CEO*. Kebijakan ini menyediakan proteksi pengguna dan domain dari peniruan lalu menerapkan kebijakan ke semua email yang diterima oleh pengguna dalam domain tersebut. Pertama, tambahkan informasi berikut ini untuk membuat kebijakan:

- **Nama**: domain dan CEO **Deskripsi**: memastikan bahwa CEO dan domain Anda tidak ditiru.
  **Diterapkan untuk**: Pilih **domain Penerima**. Di bawah **salah satu hal ini**, pilih **pilih**, lalu pilih domain. Pilih **+ Tambahkan**. Pilih kotak centang di samping nama domain dalam daftar (misalnya, *contoso.com*), lalu pilih **Tambahkan**. Pilih **selesai**.
- Setelah kebijakan dibuat, Anda dapat menyempurnakan kebijakan dengan menggunakan opsi berikut ini:
  - **Menambahkan pengguna untuk melindungi:** Untuk contoh ini, tambahkan alamat email CEO, minimal.
  - **Menambahkan domain untuk dilindungi**: Tambahkan domain organisasi yang MENYERTAKAN Office CEO.
  - **Pilih tindakan**: untuk **jika email dikirim oleh pengguna yang menyamar**, pilih **Alihkan pesan ke alamat email lain**, lalu masukkan alamat email administrator keamanan (misalnya, *securityadmin@contoso.com*). Untuk **jika email dikirim oleh domain Bersurat**, pilih **karantina pesan**.
  - **Kecerdasan kotak surat**: secara default, opsi ini dipilih saat Anda membuat kebijakan anti Pengelabuan baru. Tinggalkan **pengaturan ini** untuk hasil terbaik.
  - **Menambahkan pengirim dan domain tepercaya:** Untuk contoh ini, jangan tetapkan mengesampingkan apa pun.
- Setelah Anda meninjau pengaturan Anda, pilih **Buat kebijakan ini** atau **Simpan**, sebagaimana diperlukan.

Untuk mempelajari selengkapnya, lihat [kebijakan anti Pengelabuan di Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).
