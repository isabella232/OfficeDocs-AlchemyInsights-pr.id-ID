---
title: Mengidentifikasi kegiatan aturan kotak masuk di log audit
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1368
ms.assetid: ''
ms.openlocfilehash: 9339d9c58056f568dc994b75bffe39f2c8bbdd34
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909322"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Mengidentifikasi kegiatan aturan kotak masuk di log audit

Anda dapat menggunakan pencarian log audit di & keamanan Compliance Center untuk melihat kotak masuk aturan peristiwa (membuat, memodifikasi, dan menghapus aturan kotak masuk).

1. Masuk ke [Kantor 365 keamanan & Compliance Center](https://protection.office.com/)

2. Klik **Cari dan penyelidikan** dan pilih **Cari Log Audit**.

3. Pilih rentang tanggal di bidang **tanggal mulai** dan **tanggal akhir** .

4. Dalam **Kegiatan pertukaran kotak pesan**, pastikan bidang **kegiatan** diatur ke **New-InboxRule buat/memodifikasi/mengaktifkan/menonaktifkan aturan kotak masuk**.

5. Klik **Cari**.

Hasil, pilih catatan audit. Di flyout rincian, klik **Informasi selengkapnya**. Informasi tentang pengaturan aturan kotak masuk akan ditampilkan dalam bidang **parameter** .

Untuk informasi lebih lanjut, lihat [menentukan jika pengguna membuat aturan kotak masuk](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
