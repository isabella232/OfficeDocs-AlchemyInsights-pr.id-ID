---
title: Mengidentifikasi aktivitas aturan kotak masuk dalam log audit
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
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779054"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Mengidentifikasi aktivitas aturan kotak masuk dalam log audit

Anda dapat menggunakan pencarian log audit di pusat kepatuhan & keamanan Microsoft 365 untuk menampilkan kejadian aturan kotak masuk (membuat, mengubah, dan menghapus aturan kotak masuk).

1. Masuk ke [pusat kepatuhan & keamanan Microsoft 365](https://protection.office.com/).

2. Masuk ke halaman **Search**  >  **pencarian log audit** pencarian.

3. Pilih rentang tanggal di bidang tanggal **mulai** dan **tanggal berakhir** .

4. Di bawah **aktivitas kotak surat Exchange**, verifikasi bidang **aktivitas** diatur ke **aturan kotak masuk baru membuat/mengubah/mengaktifkan/menonaktifkan kotak masuk**.

5. Klik **Cari**.

Dalam hasil, pilih catatan audit. Dalam Flyout detail, klik **informasi selengkapnya**. Informasi tentang pengaturan aturan kotak masuk ditampilkan dalam bidang **parameter** .

Untuk informasi selengkapnya, lihat [menentukan apakah pengguna membuat aturan kotak masuk](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
