---
title: Mengidentifikasi alamat IP dan klien dalam log audit
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: e0119762d2a34bd2b0da827faf55c832e29d8a2b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539032"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Mengidentifikasi alamat IP dan klien dalam log audit

Alamat IP yang berkaitan dengan aktivitas oleh Office 365 pengguna atau administrator akan ditampilkan dalam log Audit. Informasi klien juga login. Berikut adalah langkah-langkah untuk mengidentifikasi informasi tersebut

1. Masuk ke [Kantor 365 keamanan & Compliance Center](https://protection.office.com/).

2. Pergi ke **pencarian** > halaman**pencarian log Audit** .

   Jika Anda tertarik untuk aktivitas tertentu, pilih dari daftar **kegiatan** . Jika tidak, Semua kegiatan akan dikembalikan untuk pemakai dipilih (pengaturan default).

   **Catatan**: aktivitas tertentu mungkin tidak tersedia di menu **kegiatan** ; Namun, mereka melakukan audit item akan dikembalikan jika **Menunjukkan hasil untuk semua kegiatan** adalah dipilih (pengaturan default).

3. Tentukan nama pengguna di bidang **pengguna** , pilih rentang tanggal yang tepat untuk kegiatan, dan kemudian klik **Cari**.

Hasil, Anda dapat melihat alamat IP untuk aktivitas di panel hasil. Pilih record audit untuk melihat informasi rinci di flyout **rincian** (misalnya, klien, pengguna yang melakukan tindakan, dll).

Untuk selengkapnya, lihat [mencari alamat IP komputer yang digunakan untuk mengakses account dikompromikan](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
