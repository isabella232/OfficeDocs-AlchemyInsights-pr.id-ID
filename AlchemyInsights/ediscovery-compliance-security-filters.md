---
title: Tidak ada hasil yang dikembalikan selama pencarian konten/ekspor
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/14/2020
ms.locfileid: "49678679"
---
# <a name="no-results-returned-during-content-searchexport"></a>Tidak ada hasil yang dikembalikan selama pencarian konten/ekspor

Jika Anda mengalami masalah dengan skenario eDiscovery berikut:

- Pencarian konten/ekspor mengembalikan data atau data tidak terduga
- Pencarian eDiscovery atau gagal mengekspor

Ini mungkin disebabkan karena filter keamanan kepatuhan tertentu yang disiapkan oleh admin tertentu dan tidak dikomunikasikan kepada semua admin.

Untuk mengatasi masalah ini, periksa apakah ada filter keamanan kepatuhan yang mungkin menyebabkan masalah ini:

1. Menyambungkan ke pusat keamanan dan kepatuhan PowerShell
2. Jalankan perintah berikut ini:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Untuk informasi tambahan tentang filter keamanan kepatuhan, lihat [pemfilteran izin untuk pencarian konten](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
