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
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516782"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="598fc-102">Tidak ada hasil dari konten Cari/ekspor</span><span class="sxs-lookup"><span data-stu-id="598fc-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="598fc-103">Masalah dengan konten Cari/ekspor tidak kembali data mungkin karena tertentu kepatuhan keamanan Filter itu setup oleh Admin tertentu dan tidak berkomunikasi dengan semua Admins.</span><span class="sxs-lookup"><span data-stu-id="598fc-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="598fc-104">Untuk mengatasi ini, periksa untuk melihat apakah ada filter keamanan kepatuhan yang dapat menyebabkan ini:</span><span class="sxs-lookup"><span data-stu-id="598fc-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="598fc-105">Terhubung ke keamanan dan kepatuhan pusat Powershell</span><span class="sxs-lookup"><span data-stu-id="598fc-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="598fc-106">Jalankan commandlets berikut:</span><span class="sxs-lookup"><span data-stu-id="598fc-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="598fc-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="598fc-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="598fc-108">Dapatkan-ComplianceSecurityFilter-organisasi $org</span><span class="sxs-lookup"><span data-stu-id="598fc-108">Get-ComplianceSecurityFilter -Organization $org</span></span>