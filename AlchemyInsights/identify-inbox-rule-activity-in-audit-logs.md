---
title: Mengidentifikasi aktivitas aturan kotak masuk di log audit
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f946510539b3d28f2ceeec1546cbffce8bd352fd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716427"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Mengidentifikasi aktivitas aturan kotak masuk di log audit

Anda dapat menggunakan pencarian log audit di Microsoft 365 keamanan & Compliance Center untuk melihat peristiwa aturan kotak masuk (membuat, mengubah, dan menghapus aturan kotak masuk).

1. Masuk ke [Microsoft 365 keamanan & Compliance Center](https://protection.office.com/).

2. Buka halaman pencarian **Search** > **log audit** penelusuran.

3. Pilih rentang tanggal di kolom tanggal **mulai** dan **tanggal akhir** .

4. Di bawah **kotak surat Exchange aktivitas**, verifikasi kolom **aktivitas** diatur ke **baru-inboxrule membuat/mengubah/mengaktifkan/menonaktifkan aturan kotak masuk**.

5. Klik **Cari**.

Di hasil, pilih rekaman audit. Dalam Flyout rincian, klik **informasi lebih lanjut**. Informasi tentang pengaturan aturan kotak masuk ditampilkan di bidang **parameter** .

Untuk informasi lebih lanjut, lihat [menentukan apakah pengguna membuat aturan kotak masuk](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
