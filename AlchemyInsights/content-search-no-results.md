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
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="a2029-102">Tidak ada hasil dari konten Cari/ekspor</span><span class="sxs-lookup"><span data-stu-id="a2029-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="a2029-103">Masalah dengan konten Cari/ekspor tidak kembali data mungkin karena tertentu kepatuhan keamanan Filter itu setup oleh Admin tertentu dan tidak berkomunikasi dengan semua Admins.</span><span class="sxs-lookup"><span data-stu-id="a2029-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="a2029-104">Untuk mengatasi ini, periksa untuk melihat apakah ada filter keamanan kepatuhan yang dapat menyebabkan ini:</span><span class="sxs-lookup"><span data-stu-id="a2029-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="a2029-105">Terhubung ke keamanan dan kepatuhan pusat Powershell</span><span class="sxs-lookup"><span data-stu-id="a2029-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="a2029-106">Jalankan commandlets berikut:</span><span class="sxs-lookup"><span data-stu-id="a2029-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="a2029-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="a2029-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="a2029-108">Dapatkan-ComplianceSecurityFilter-organisasi $org</span><span class="sxs-lookup"><span data-stu-id="a2029-108">Get-ComplianceSecurityFilter -Organization $org</span></span>