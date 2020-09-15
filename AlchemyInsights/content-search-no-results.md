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
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="8a440-102">Tidak ada hasil dari pencarian konten/ekspor</span><span class="sxs-lookup"><span data-stu-id="8a440-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="8a440-103">Masalah dengan pencarian konten/ekspor tidak mengembalikan data apa pun mungkin karena filter keamanan kepatuhan tertentu yang disiapkan oleh admin tertentu dan tidak mengkomunikinya ke semua admin.</span><span class="sxs-lookup"><span data-stu-id="8a440-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="8a440-104">Untuk mengatasi masalah ini, periksa apakah ada filter keamanan kepatuhan yang mungkin menyebabkan hal ini:</span><span class="sxs-lookup"><span data-stu-id="8a440-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="8a440-105">Menyambungkan ke pusat keamanan dan kepatuhan PowerShell</span><span class="sxs-lookup"><span data-stu-id="8a440-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="8a440-106">Jalankan perintah berikut ini:</span><span class="sxs-lookup"><span data-stu-id="8a440-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="8a440-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="8a440-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="8a440-108">Get-ComplianceSecurityFilter-$org organisasi</span><span class="sxs-lookup"><span data-stu-id="8a440-108">Get-ComplianceSecurityFilter -Organization $org</span></span>