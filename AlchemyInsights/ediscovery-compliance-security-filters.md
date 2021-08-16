---
title: Tidak ada hasil yang dikembalikan selama Pencarian/Ekspor Konten
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
ms.openlocfilehash: 5c04364f98dccbcad0f011df866f137d79c166ad3839b408d6be447d50a87ac3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101269"
---
# <a name="no-results-returned-during-content-searchexport"></a>Tidak ada hasil yang dikembalikan selama Pencarian/Ekspor Konten

Jika Anda mengalami masalah dengan skenario eDiscovery berikut ini:

- Pencarian/Ekspor Konten tidak mengembalikan data atau data yang tidak diharapkan
- Pencarian eDiscovery atau Ekspor gagal

Hal ini mungkin terjadi karena Filter Keamanan Kepatuhan tertentu yang disiapkan oleh Admin tertentu dan belum dikomunikasikan ke semua Admin.

Untuk mengatasi ini, periksa apakah ada Filter Keamanan Kepatuhan apa pun yang mungkin menyebabkan masalah ini:

1. Koneksi ke Powershell Pusat Keamanan dan Kepatuhan
2. Jalankan commandlet berikut:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Untuk informasi tambahan tentang Filter Keamanan Kepatuhan, lihat [Pemfilteran Izin untuk Pencarian Konten](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
