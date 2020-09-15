---
title: Pencarian konten tidak ada hasil
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680650"
---
# <a name="no-results-from-content-searchexports"></a>Tidak ada hasil dari pencarian konten/ekspor

Masalah dengan pencarian konten/ekspor tidak mengembalikan data apa pun mungkin karena filter keamanan kepatuhan tertentu yang disiapkan oleh admin tertentu dan tidak mengkomunikinya ke semua admin.

Untuk mengatasi masalah ini, periksa apakah ada filter keamanan kepatuhan yang mungkin menyebabkan hal ini:
1. Menyambungkan ke pusat keamanan dan kepatuhan PowerShell
2. Jalankan perintah berikut ini:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-$org organisasi