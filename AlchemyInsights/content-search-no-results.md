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
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="3c279-102">Tidak ada hasil dari Pencarian/Ekspor Konten</span><span class="sxs-lookup"><span data-stu-id="3c279-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="3c279-103">Masalah terkait Pencarian/Ekspor Konten yang tidak mengembalikan data apa pun mungkin disebabkan oleh Filter Keamanan Kepatuhan tertentu yang disiapkan oleh Admin tertentu dan tidak mengkomunikasikannya ke semua Admin.</span><span class="sxs-lookup"><span data-stu-id="3c279-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="3c279-104">Untuk mengatasi masalah ini, periksalah untuk melihat apakah ada Filter Keamanan Kepatuhan yang mungkin menyebabkan ini:</span><span class="sxs-lookup"><span data-stu-id="3c279-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="3c279-105">Menyambungkan ke Powershell Pusat Keamanan dan Kepatuhan</span><span class="sxs-lookup"><span data-stu-id="3c279-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="3c279-106">Jalankan commandlet berikut:</span><span class="sxs-lookup"><span data-stu-id="3c279-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="3c279-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="3c279-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="3c279-108">Get-ComplianceSecurityFilter -Organization $org</span><span class="sxs-lookup"><span data-stu-id="3c279-108">Get-ComplianceSecurityFilter -Organization $org</span></span>