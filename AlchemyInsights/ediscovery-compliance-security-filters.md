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
ms.openlocfilehash: 8786f11f170edb151879235e19caa38b50f3f06e
ms.sourcegitcommit: 3d662e1a1440ba74b5347896347d03bb8c8f3af5
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/22/2020
ms.locfileid: "49727226"
---
# <a name="no-results-returned-during-content-searchexport"></a>Tidak ada hasil yang dikembalikan selama pencarian konten/ekspor

Jika Anda mengalami masalah dengan skenario eDiscovery berikut:

- Pencarian konten/ekspor mengembalikan data atau data tidak terduga
- Pencarian eDiscovery atau gagal mengekspor

Ini mungkin disebabkan oleh filter keamanan kepatuhan tertentu yang disiapkan oleh admin tertentu dan tidak dikomunikasikan kepada semua admin.

Untuk mengatasi masalah ini, periksa apakah ada filter keamanan kepatuhan yang mungkin menyebabkan masalah ini:

1. Menyambungkan ke pusat keamanan dan kepatuhan PowerShell
2. Jalankan perintah berikut ini:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Untuk informasi tambahan tentang filter keamanan kepatuhan, lihat [pemfilteran izin untuk pencarian konten](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
