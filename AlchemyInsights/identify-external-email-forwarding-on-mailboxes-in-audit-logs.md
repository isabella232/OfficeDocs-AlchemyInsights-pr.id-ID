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
ms.openlocfilehash: b7146b2b09b6ac1e33b192dcbcbfb72ea2593313
ms.sourcegitcommit: 89d938a2d402791ae66dddadba3063e9418f48cb
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/28/2021
ms.locfileid: "53630252"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Mengidentifikasi saat penerusan email eksternal dikonfigurasi pada kotak surat

Jika pengguna Microsoft 365 mengonfigurasi penerusan email eksternal di kotak surat, aktivitas akan diaudit sebagai bagian dari cmdlet **Set-Mailbox.** Anda dapat melihat aktivitas menggunakan pencarian log audit di Pusat & Kepatuhan Keamanan.

1. Masuk ke pusat [Microsoft 365 Kepatuhan Anda.](https://protection.office.com/)

2. Masuk ke halaman **pencarian**  >  **log Pencarian** audit.

3. Pilih rentang tanggal di bidang **Tanggal mulai** **dan Tanggal** selesai. Anda tidak perlu menentukan nama pengguna. Verifikasi bahwa **bidang** Aktivitas diatur ke **Perlihatkan hasil untuk semua aktivitas.**

4. Klik **Cari.**

Dalam hasil, klik **Filter Hasil,** lalu ketikkan **Set-Mailbox** dalam kotak filter aktivitas. Pilih catatan audit dalam hasil. Di **flyout** Detail, klik **Informasi selengkapnya.** Anda harus melihat detail setiap catatan audit untuk mengetahui apakah aktivitas tersebut terkait dengan penerusan email.

- **ObjectId**: Nilai alias kotak surat yang telah dimodifikasi.

- **Parameter**: _ForwardingSmtpAddress_ menunjukkan alamat email target.

- **UserId**: Pengguna yang mengonfigurasi penerusan email pada kotak surat di bidang **ObjectId.**

Untuk informasi selengkapnya, [lihat Menentukan siapa yang menyiapkan penerusan email untuk kotak surat](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
