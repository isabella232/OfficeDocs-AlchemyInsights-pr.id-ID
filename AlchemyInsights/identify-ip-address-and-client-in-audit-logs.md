---
title: Mengidentifikasi alamat IP dan klien dalam log audit
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 80b652eb65612093252dee226a19ec74bc035faa
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508919"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Mengidentifikasi alamat IP dan klien dalam log audit

Alamat IP yang berkaitan dengan aktivitas oleh pengguna 365 Microsoft atau administrator ditampilkan di log audit. Informasi klien juga dicatat. Berikut adalah langkah untuk mengidentifikasi informasi tersebut

1. Masuk ke [Microsoft 365 keamanan & Compliance Center](https://protection.office.com/).

2. Buka halaman penelusuran **Search**  >  **log audit** penelusuran.

   Jika Anda tertarik dengan aktivitas tertentu, pilih dari daftar **aktivitas** . Jika tidak, semua aktivitas akan dikembalikan untuk pengguna yang dipilih (setelan default).

   **Catatan**: aktivitas tertentu mungkin tidak tersedia di menu **aktivitas** ; Namun, item audit tersebut akan dikembalikan jika **Tampilkan hasil untuk semua aktivitas** dipilih (pengaturan default).

3. Tentukan nama pengguna di bidang **pengguna** , pilih rentang tanggal yang sesuai untuk aktivitas, dan kemudian klik **Cari**.

Pada hasil, Anda dapat melihat alamat IP untuk aktivitas tersebut di panel hasil. Pilih rekaman audit untuk melihat informasi terperinci dalam Flyout **rincian** (misalnya, klien, pengguna yang melakukan tindakan, dsb.).

Untuk informasi lebih lanjut, lihat [menemukan alamat IP komputer yang digunakan untuk mengakses akun yang disusupi](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
