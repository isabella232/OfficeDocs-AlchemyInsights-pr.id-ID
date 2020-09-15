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
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696300"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Mengidentifikasi Kapan penerusan email eksternal dikonfigurasikan pada kotak surat

Saat pengguna Microsoft 365 mengonfigurasi penerusan email eksternal pada kotak surat, aktivitas diaudit sebagai bagian dari cmdlet **Set-Mailbox** . Anda dapat melihat aktivitas menggunakan pencarian log audit di pusat kepatuhan & keamanan.

1. Masuk ke [pusat kepatuhan & keamanan Microsoft 365](https://protection.office.com/).

2. Masuk ke halaman **Search**  >  **pencarian log audit** pencarian.

3. Pilih rentang tanggal di bidang tanggal **mulai** dan **tanggal berakhir** . Anda tidak perlu menentukan nama pengguna. Verifikasi bidang **aktivitas** diatur untuk **memperlihatkan hasil untuk semua aktivitas**.

4. Klik **Cari**.

Dalam hasil, klik **filter hasil** dan ketik **set-kotak surat** di kotak filter aktivitas. Pilih catatan audit dalam hasil. Dalam Flyout **detail** , klik **informasi selengkapnya**. Anda harus melihat detail setiap catatan audit untuk menentukan apakah aktivitas terkait dengan penerusan email.

- **ObjectID**: nilai alias dari kotak surat yang telah dimodifikasi.

- **Parameter**: _forwardingsmtpaddress_ menunjukkan alamat email target.

- **Userid**: pengguna yang mengonfigurasikan penerusan email pada kotak surat di bidang **ObjectID** .

Untuk informasi selengkapnya, lihat [menentukan siapa yang menyetel penerusan email untuk kotak surat](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
