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
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/14/2020
ms.locfileid: "49678679"
---
# <a name="no-results-returned-during-content-searchexport"></a><span data-ttu-id="f3b23-102">Tidak ada hasil yang dikembalikan selama pencarian konten/ekspor</span><span class="sxs-lookup"><span data-stu-id="f3b23-102">No results returned during Content Search/Export</span></span>

<span data-ttu-id="f3b23-103">Jika Anda mengalami masalah dengan skenario eDiscovery berikut:</span><span class="sxs-lookup"><span data-stu-id="f3b23-103">If you are experiencing issues with the following eDiscovery scenarios:</span></span>

- <span data-ttu-id="f3b23-104">Pencarian konten/ekspor mengembalikan data atau data tidak terduga</span><span class="sxs-lookup"><span data-stu-id="f3b23-104">Content Search/Export returns no data or unexpected data</span></span>
- <span data-ttu-id="f3b23-105">Pencarian eDiscovery atau gagal mengekspor</span><span class="sxs-lookup"><span data-stu-id="f3b23-105">eDiscovery Search or Export fails</span></span>

<span data-ttu-id="f3b23-106">Ini mungkin disebabkan karena filter keamanan kepatuhan tertentu yang disiapkan oleh admin tertentu dan tidak dikomunikasikan kepada semua admin.</span><span class="sxs-lookup"><span data-stu-id="f3b23-106">This may be caused due to certain Compliance Security Filters that were setup by a specific Admin and not been communicated to all Admins.</span></span>

<span data-ttu-id="f3b23-107">Untuk mengatasi masalah ini, periksa apakah ada filter keamanan kepatuhan yang mungkin menyebabkan masalah ini:</span><span class="sxs-lookup"><span data-stu-id="f3b23-107">To resolve this, check if there are any Compliance Security Filters that may be causing these issues:</span></span>

1. <span data-ttu-id="f3b23-108">Menyambungkan ke pusat keamanan dan kepatuhan PowerShell</span><span class="sxs-lookup"><span data-stu-id="f3b23-108">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="f3b23-109">Jalankan perintah berikut ini:</span><span class="sxs-lookup"><span data-stu-id="f3b23-109">Run the following commandlets:</span></span>

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

<span data-ttu-id="f3b23-110">Untuk informasi tambahan tentang filter keamanan kepatuhan, lihat [pemfilteran izin untuk pencarian konten](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span><span class="sxs-lookup"><span data-stu-id="f3b23-110">For additional information on Compliance Security Filters, see [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span></span>
