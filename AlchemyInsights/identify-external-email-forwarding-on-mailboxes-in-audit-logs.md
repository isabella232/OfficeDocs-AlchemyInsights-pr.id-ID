---
title: Mengidentifikasi penerusan email eksternal pada kotak surat dalam log audit
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 48634fad8f573e3a7c38cac299bb95ec90814f5c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331162"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Mengidentifikasi saat penerusan email eksternal dikonfigurasi pada kotak surat

Jika pengguna Microsoft 365 mengonfigurasi penerusan email eksternal di kotak surat, aktivitas akan diaudit sebagai bagian dari cmdlet **Set-Mailbox.** Anda dapat melihat aktivitas menggunakan pencarian log audit. Berikut cara melakukannya.

1. Lakukan salah satu langkah berikut ini:
   - Pada bagian pusat kepatuhan Microsoft 365 <https://compliance.microsoft.com> , masuk ke **Audit** \> **Solusi**. Atau, untuk langsung masuk ke **halaman Audit,** gunakan <https://compliance.microsoft.com/auditlogsearch> .
   - Di portal Pertahanan Microsoft 365 di <https://security.microsoft.com> , masuk ke **Audit**. Atau, untuk langsung masuk ke **halaman Audit,** gunakan <https://sip.security.microsoft.com/auditlogsearch> .

2. Pada halaman **Audit,** verifikasi bahwa tab **Pencarian** dipilih lalu konfigurasi pengaturan berikut ini:
   - Pilih rentang tanggal/waktu dalam kotak **Mulai** **dan** Akhir.
   - Verifikasi kotak **Aktivitas** berisi **Perlihatkan hasil untuk semua aktivitas.**

3. Bila Anda sudah selesai, klik **Cari.** Aktivitas akan muncul di halaman **Pencarian audit baru.**

4. Dalam hasil, klik **Filter Hasil,** lalu ketikkan **Set-Mailbox** dalam kotak filter aktivitas.

5. Pilih catatan audit dalam hasil. Di **flyout** Detail, klik **Informasi selengkapnya.** Anda perlu melihat detail setiap catatan audit untuk menentukan apakah aktivitas tersebut terkait dengan penerusan email.

   - **ObjectId**: Nilai alias kotak surat yang telah dimodifikasi.
   - **Parameter**: _ForwardingSmtpAddress_ menunjukkan alamat email target.
   - **UserId**: Pengguna yang mengonfigurasi penerusan email pada kotak surat di bidang **ObjectId.**

Untuk informasi selengkapnya, [lihat Menentukan siapa yang menyiapkan penerusan email untuk kotak surat](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
