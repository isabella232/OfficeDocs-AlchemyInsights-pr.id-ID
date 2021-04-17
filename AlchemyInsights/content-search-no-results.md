---
title: Pencarian Konten Tidak Ada Hasil
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816851"
---
# <a name="no-results-from-content-searchexports"></a>Tidak ada hasil dari Pencarian/Ekspor Konten

Masalah terkait Pencarian/Ekspor Konten yang tidak mengembalikan data apa pun mungkin disebabkan oleh Filter Keamanan Kepatuhan tertentu yang disiapkan oleh Admin tertentu dan tidak mengkomunikasikannya ke semua Admin.

Untuk mengatasi masalah ini, periksalah untuk melihat apakah ada Filter Keamanan Kepatuhan yang mungkin menyebabkan ini:
1. Menyambungkan ke Powershell Pusat Keamanan dan Kepatuhan
2. Jalankan commandlet berikut:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organization $org