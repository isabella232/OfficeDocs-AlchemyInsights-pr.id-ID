---
title: Mengidentifikasi penerusan email eksternal pada kotak pesan di log audit
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1369
ms.assetid: ''
ms.openlocfilehash: 7fb2c161c558a7eb961f86ca2b86e33750d902fd
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/23/2019
ms.locfileid: "32417215"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Mengidentifikasi ketika penerusan email eksternal dikonfigurasi pada kotak pesan

Ketika pengguna mengkonfigurasi penerusan email eksternal di kotak pesan, kegiatan audit sebagai bagian dari cmdlet **Set-Mailbox** . Anda dapat melihat aktivitas yang menggunakan log audit pencarian di & keamanan Compliance Center.

1. Masuk ke [Kantor 365 keamanan & Compliance Center](https://protection.office.com/)

2. Klik **Cari dan penyelidikan** dan pilih **Cari Log Audit**.

3. Pilih rentang tanggal di bidang **tanggal mulai** dan **tanggal akhir** . Anda tidak perlu menetapkan nama pengguna. Pastikan bidang **kegiatan** diatur untuk **menunjukkan hasil untuk semua kegiatan**.

4. Klik **Cari**.

Hasil, klik **Filter hasil** dan ketik **Set-kotak surat** di kotak filter aktivitas. Pilih record audit dalam hasil. Di flyout **rincian** , klik **informasi lebih lanjut**. Anda harus melihat pada rincian dari setiap record audit untuk menentukan jika aktivitas terkait dengan email forwarding.

- **ObjectId**: nilai alias kotak pesan yang diubah.

- **Parameter**: _ForwardingSmtpAddress_ menunjukkan alamat email target.

- **UserId**: pengguna yang dikonfigurasi pengalihan email di kotak surat di bidang **ObjectId** .

Untuk informasi lebih lanjut, lihat [menentukan yang mengatur email forwarding untuk kotak pesan](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
