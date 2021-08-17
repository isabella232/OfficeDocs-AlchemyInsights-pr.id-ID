---
title: Mengidentifikasi alamat IP dan klien dalam log audit
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
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 57a1756787f8297a2a1ab3012b95aaa2f33e6045
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/13/2021
ms.locfileid: "58313022"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Mengidentifikasi alamat IP dan klien dalam log audit

Alamat IP yang berkaitan dengan aktivitas oleh Microsoft 365 atau administrator diperlihatkan dalam Log Audit. Informasi klien juga dicatat. Berikut langkah-langkah untuk mengidentifikasi informasi tersebut

1. Masuk ke pusat [Microsoft 365 Kepatuhan Anda.](https://protection.office.com/)

2. Masuk ke halaman **pencarian**  >  **log Pencarian** audit.

   Jika Anda tertarik pada aktivitas tertentu, pilih aktivitas tersebut dari **daftar** Aktivitas. Jika tidak, semua aktivitas akan dikembalikan untuk pengguna yang dipilih (pengaturan default).

   **Catatan**: Aktivitas tertentu mungkin tidak tersedia **di** menu Aktivitas; namun, item audit tersebut akan dikembalikan jika **Perlihatkan Hasil untuk semua aktivitas** dipilih (pengaturan default).

3. Tentukan nama pengguna di **bidang** Pengguna, pilih rentang tanggal yang sesuai untuk aktivitas tersebut, lalu klik **Cari.**

Dalam hasil, Anda dapat melihat alamat IP untuk aktivitas tersebut di panel hasil. Pilih catatan audit untuk melihat informasi mendetail dalam **flyout** Detail (misalnya, Klien, Pengguna yang melakukan tindakan, dll.).

Untuk informasi selengkapnya, [lihat Menemukan alamat IP komputer yang digunakan untuk mengakses akun dibobol.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account)
