---
title: Cari tahu siapa yang menyiapkan penerusan di kotak surat, dan caranya
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
ms.openlocfilehash: d6be4331967ed9ae362f5da85856b03cfa40b319
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317811"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Cari tahu siapa yang menyiapkan penerusan di kotak surat, dan caranya

Jika penerusan eksternal diatur di kotak surat, aktivitas akan diaudit sebagai bagian dari cmdlet **Set-Mailbox.** Berikut cara menemukan aktivitas dalam log audit:

1. Lakukan salah satu tindakan berikut ini:
   - Pada bagian pusat kepatuhan Microsoft 365 <https://compliance.microsoft.com> , masuk ke **Audit** \> **Solusi**. Atau, untuk langsung masuk ke **halaman Audit,** gunakan <https://compliance.microsoft.com/auditlogsearch> .
   - Di portal Pertahanan Microsoft 365 di <https://security.microsoft.com> , masuk ke **Audit**. Atau, untuk langsung masuk ke **halaman Audit,** gunakan <https://security.microsoft.com/auditlogsearch> .

   **Catatan**: Jika melihat pemberitahuan bahwa Anda perlu mengaktifkan pengauditan, lanjutkan dan aktifkan sekarang. Jika fitur ini tidak diaktifkan, hasil pencarian tidak akan dapat mengambil data dari tanggal sebelumnya.

2. Pada halaman **Audit,** verifikasi bahwa tab **Pencarian** dipilih lalu konfigurasi pengaturan berikut ini:
   - Pilih rentang tanggal/waktu dalam kotak **Mulai** **dan** Akhir.
   - Verifikasi kotak **Aktivitas** berisi **Perlihatkan hasil untuk semua aktivitas.**

3. Bila Anda sudah selesai, klik **Cari.** Aktivitas akan muncul di halaman **Pencarian audit baru.**

4. Dalam hasil, klik kolom **Aktivitas** untuk mengurutkan hasil, dan cari entri **Set-Mailbox.**

5. Pilih aktivitas dalam hasil untuk membuka flyout detail. Anda perlu melihat detail setiap catatan audit untuk mengetahui apakah aktivitas terkait dengan penerusan email:
   - **ObjectId**: Nilai alias kotak surat yang telah dimodifikasi.
   - **Parameter**: _ForwardingSmtpAddress_ menunjukkan alamat email target.
   - **UserId**: Pengguna yang mengonfigurasi penerusan email pada kotak surat di bidang **ObjectId.**

Untuk informasi selengkapnya, [lihat Menentukan siapa yang menyiapkan penerusan email untuk kotak surat](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
