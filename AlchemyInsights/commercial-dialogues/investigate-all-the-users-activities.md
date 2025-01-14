---
title: Selidiki semua aktivitas pengguna
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 016f4b1caa05cb26d1e6795551b64737d4cb64a5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332346"
---
# <a name="investigate-all-the-users-activities"></a>Selidiki semua aktivitas pengguna

Berikut cara melakukannya:

1. Lakukan salah satu tindakan berikut ini:
   - Pada bagian pusat kepatuhan Microsoft 365 <https://compliance.microsoft.com> , masuk ke **Audit** \> **Solusi**. Atau, untuk langsung masuk ke **halaman Audit,** gunakan <https://compliance.microsoft.com/auditlogsearch> .
   - Di portal Pertahanan Microsoft 365 di <https://security.microsoft.com> , masuk ke **Audit**. Atau, untuk langsung masuk ke **halaman Audit,** gunakan <https://security.microsoft.com/auditlogsearch> .

    **Catatan**: Jika Anda melihat pemberitahuan bahwa Anda perlu mengaktifkan fitur, lanjutkan dan aktifkan sekarang. Jika fitur tidak diaktifkan, hasil pencarian tidak akan dapat menarik data dari tanggal sebelumnya.

2. Pada tab **Pencarian** dari halaman **Audit,** konfigurasi pengaturan berikut ini:
   - **Rentang tanggal dan waktu**: Pilih rentang tanggal/waktu dalam **kotak** Mulai **dan** Akhir.
   - **Aktivitas**: Jika Anda tertarik dengan aktivitas tertentu, pilih aktivitas tersebut dari daftar; jika tidak, nilai default **Perlihatkan hasil untuk semua aktivitas** mengembalikan semua aktivitas.
   - **Pengguna**: Terima nilai default kosong untuk mengembalikan hasil bagi semua pengguna, atau masukkan satu atau beberapa pengguna.

3. Bila Anda sudah selesai, klik **Cari.** Aktivitas akan muncul di halaman **Pencarian audit baru.** Anda akan melihat alamat **IP ,** **Pengguna**, dan **nama** Aktivitas.

4. Untuk mengunduh hasil,  pilih Ekspor \> **Unduh semua Hasil.**

5. Pilih aktivitas dalam hasil untuk membuka flyout detail.

Untuk mempelajari selengkapnya, lihat [Mencari log audit untuk menyelidiki masalah dukungan umum.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
