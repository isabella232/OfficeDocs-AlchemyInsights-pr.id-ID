---
title: Masalah kinerja-SharePoint atau OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068408"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="1b5fb-102">SharePoint atau OneDrive lambat, tidak dapat diakses, atau tidak tersedia untuk beberapa pengguna</span><span class="sxs-lookup"><span data-stu-id="1b5fb-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="1b5fb-103">SharePoint atau OneDrive mungkin lambat, tidak dapat diakses, atau tidak tersedia, atau mungkin menampilkan layanan tidak tersedia atau 503 kesalahan, karena beberapa alasan:</span><span class="sxs-lookup"><span data-stu-id="1b5fb-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="1b5fb-104">Jika situs SharePoint atau OneDrive lambat atau tertunda untuk beberapa pengguna, mungkin ada masalah layanan sementara di mana pengguna mengalami penundaan terputus-putus atau galat navigasi ketika mengakses situs SharePoint atau konten OneDrive.</span><span class="sxs-lookup"><span data-stu-id="1b5fb-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="1b5fb-105">Periksa [dasbor Kesehatan Layanan](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) untuk melihat apakah organisasi Anda terpengaruh.</span><span class="sxs-lookup"><span data-stu-id="1b5fb-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="1b5fb-106">Pengguna akan menerima *503 server sibuk* galat saat berusaha menavigasi ke situs SharePoint atau OneDrive.</span><span class="sxs-lookup"><span data-stu-id="1b5fb-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="1b5fb-107">Galat ini dapat disebabkan oleh pelambatan dalam Layanan SharePoint.</span><span class="sxs-lookup"><span data-stu-id="1b5fb-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="1b5fb-108">SharePoint Online menggunakan pelambatan untuk mempertahankan kinerja optimal dan keandalan Layanan SharePoint online.</span><span class="sxs-lookup"><span data-stu-id="1b5fb-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="1b5fb-109">Pelambatan membatasi jumlah tindakan pengguna atau panggilan bersamaan (dengan skrip atau kode) untuk mencegah penggunaan sumber daya berlebihan.</span><span class="sxs-lookup"><span data-stu-id="1b5fb-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="1b5fb-110">Untuk informasi lebih lanjut tentang pelambatan Lihat, [Hindari mendapatkan mengalami kelambatan atau diblokir di SharePoint online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="1b5fb-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="1b5fb-111">Jika Anda mengalami kinerja yang lambat dengan situs atau halaman SharePoint **klasik** atau **modern** , gunakan [alat diagnostik halaman](https://aka.ms/perftool) untuk menganalisis halaman.</span><span class="sxs-lookup"><span data-stu-id="1b5fb-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="1b5fb-112">Jika Anda masih mengalami kinerja lambat umum, Tinjau sumber daya di bagian bawah artikel ini: [pengantar tuning kinerja untuk SharePoint online](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="1b5fb-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  