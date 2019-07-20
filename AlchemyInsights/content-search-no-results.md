---
title: Konten tidak hasil pencarian
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800410"
---
# <a name="no-results-from-content-searchexports"></a>Tidak ada hasil dari konten Cari/ekspor

Masalah dengan konten Cari/ekspor tidak kembali data mungkin karena tertentu kepatuhan keamanan Filter itu setup oleh Admin tertentu dan tidak berkomunikasi dengan semua Admins.

Untuk mengatasi ini, periksa untuk melihat apakah ada filter keamanan kepatuhan yang dapat menyebabkan ini:
1. Terhubung ke keamanan dan kepatuhan pusat Powershell
2. Jalankan commandlets berikut:
<br>$org = "yourdomain.com"
<br>Dapatkan-ComplianceSecurityFilter-organisasi $org