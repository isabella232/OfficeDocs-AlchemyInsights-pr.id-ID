---
title: Menemukan alamat IP di log audit
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: c3b1cac5379f4f3da93152fa20086068f7df562cd98b2980ce1b4280e0aa6d5f
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/11/2021
ms.locfileid: "57902263"
---
# <a name="find-the-ip-address-in-audit-log"></a>Menemukan alamat IP di log audit

Alamat IP yang berkaitan dengan aktivitas yang dilakukan oleh pengguna atau administrator diperlihatkan dalam log audit. Informasi klien juga dicatat. Berikut cara mengidentifikasi alamat IP tersebut:

1. Lakukan salah satu tindakan berikut ini:
   - Pada bagian pusat kepatuhan Microsoft 365 <https://compliance.microsoft.com> , masuk ke **Audit** \> **Solusi**. Atau, untuk langsung masuk ke **halaman Audit,** gunakan <https://compliance.microsoft.com/auditlogsearch> .
   - Pada portal Pertahanan Microsoft 365 di <https://security.microsoft.com> , masuk ke **Audit**. Atau, untuk langsung masuk ke **halaman Audit,** gunakan <https://security.microsoft.com/auditlogsearch> .

    > [!NOTE]
    > Jika melihat pemberitahuan bahwa Anda perlu mengaktifkan pengauditan, lanjutkan dan aktifkan sekarang. Jika fitur ini tidak diaktifkan, hasil pencarian tidak akan dapat mengambil data dari tanggal sebelumnya.

2. Pada halaman **Audit,** verifikasi bahwa tab **Pencarian** dipilih lalu konfigurasi pengaturan berikut ini:
   - **Rentang tanggal dan waktu**: Pilih rentang tanggal/waktu dalam **kotak** Mulai **dan** Akhir.
   - **Aktivitas**: Jika Anda tertarik dengan aktivitas tertentu, pilih aktivitas tersebut dari daftar; jika tidak, nilai default **Perlihatkan hasil untuk semua** aktivitas mengembalikan semua aktivitas.. Perhatikan bahwa aktivitas tertentu mungkin tidak tersedia untuk dipilih; namun, item audit tersebut akan dikembalikan jika **Perlihatkan hasil untuk semua** aktivitas dipilih.
   - **Pengguna**: Terima nilai default kosong untuk mengembalikan hasil bagi semua pengguna, atau masukkan satu atau beberapa pengguna.

3. Bila Anda sudah selesai, klik **Cari.** Aktivitas akan muncul di halaman **Pencarian audit baru.**

4. Dalam hasil, klik **Filter Hasil,** lalu ketikkan **Set-Mailbox** dalam kotak filter aktivitas.

5. Pilih catatan audit dalam hasil untuk membuka **flyout** Detail.

Untuk informasi selengkapnya, lihat [Mencari log audit untuk menyelidiki masalah dukungan umum.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
