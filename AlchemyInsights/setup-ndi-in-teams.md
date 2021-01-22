---
title: Mengaktifkan teknologi NDI
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
- "9004403"
- "7947"
ms.openlocfilehash: ea694898baffa50fca71957175eba3664dece44e
ms.sourcegitcommit: 112f18dce8257b98fab32d44910ee879efb44cb8
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935130"
---
# <a name="turn-on-ndi-technology"></a><span data-ttu-id="7d5fd-102">Mengaktifkan teknologi NDI</span><span class="sxs-lookup"><span data-stu-id="7d5fd-102">Turn on NDI technology</span></span>

<span data-ttu-id="7d5fd-103">Teknologi NDI memerlukan dua langkah untuk diaktifkan untuk pengguna:</span><span class="sxs-lookup"><span data-stu-id="7d5fd-103">NDI technology requires two steps to be turned on for a user:</span></span>

1. <span data-ttu-id="7d5fd-104">Admin penyewa harus mengaktifkan properti ' AllowNDIStreaming ' di CsTeamsMeetingPolicy.</span><span class="sxs-lookup"><span data-stu-id="7d5fd-104">The tenant admin must enable the 'AllowNDIStreaming' property in CsTeamsMeetingPolicy.</span></span>

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. <span data-ttu-id="7d5fd-105">Setelah perubahan ini diisi, pengguna akhir harus mengaktifkan teknologi® NDI untuk klien tertentu dari **pengaturan > izin**.</span><span class="sxs-lookup"><span data-stu-id="7d5fd-105">After this change has populated, the end user must turn on NDI® technology for their specific client from **Settings > Permissions**.</span></span>

<span data-ttu-id="7d5fd-106">Untuk informasi selengkapnya, lihat [menggunakan teknologi NDI di Microsoft teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).</span><span class="sxs-lookup"><span data-stu-id="7d5fd-106">For more information, see [Use NDI technology in Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).</span></span>
