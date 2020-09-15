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
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668313"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Mengidentifikasi alamat IP dan klien dalam log audit

Alamat IP yang terkait dengan aktivitas oleh pengguna atau administrator Microsoft 365 diperlihatkan dalam log audit. Informasi klien juga dicatat. Berikut adalah langkah-langkah untuk mengidentifikasi informasi tersebut

1. Masuk ke [pusat kepatuhan & keamanan Microsoft 365](https://protection.office.com/).

2. Masuk ke halaman **Search**  >  **pencarian log audit** pencarian.

   Jika Anda tertarik dengan aktivitas tertentu, pilih dari daftar **aktivitas** . Jika tidak, semua aktivitas akan dikembalikan untuk pengguna yang dipilih (pengaturan default).

   **Catatan**: aktivitas tertentu mungkin tidak tersedia di menu **aktivitas** ; Namun, item audit tersebut akan dikembalikan jika **memperlihatkan hasil untuk semua aktivitas** yang dipilih (pengaturan default).

3. Tentukan nama pengguna di bidang **pengguna** , pilih rentang tanggal yang sesuai untuk aktivitas tersebut, lalu klik **Cari**.

Dalam hasil, Anda dapat melihat alamat IP untuk aktivitas tersebut di panel hasil. Pilih catatan audit untuk melihat informasi mendetail dalam Flyout **detail** (misalnya, klien, pengguna yang melakukan tindakan, dsb.).

Untuk informasi selengkapnya, lihat [menemukan alamat IP komputer yang digunakan untuk mengakses akun yang dikompromikan](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
