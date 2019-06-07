---
title: Mengidentifikasi kegiatan aturan kotak masuk di log audit
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1368
ms.assetid: ''
ms.openlocfilehash: f130846dd24cef81177934aa2a200c1056172d3f
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/07/2019
ms.locfileid: "34755041"
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
