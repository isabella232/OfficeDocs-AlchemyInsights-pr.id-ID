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
ms.openlocfilehash: b53534dd0666fa64e692910aa6800abab30169a97fbe567c815ce6b948381a63
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058005"
---
# <a name="no-results-from-content-searchexports"></a>Tidak ada hasil dari Pencarian/Ekspor Konten

Masalah terkait Pencarian/Ekspor Konten yang tidak mengembalikan data apa pun mungkin disebabkan oleh Filter Keamanan Kepatuhan tertentu yang disiapkan oleh Admin tertentu dan tidak mengkomunikasikannya ke semua Admin.

Untuk mengatasi masalah ini, periksalah untuk melihat apakah ada Filter Keamanan Kepatuhan yang mungkin menyebabkan ini:
1. Koneksi ke Powershell Pusat Keamanan dan Kepatuhan
2. Jalankan commandlet berikut:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organization $org