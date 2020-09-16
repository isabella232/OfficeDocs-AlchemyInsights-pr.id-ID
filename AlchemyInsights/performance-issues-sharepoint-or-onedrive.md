---
title: Masalah kinerja-SharePoint atau OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771904"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="03133-102">SharePoint atau OneDrive lambat, tidak dapat diakses, atau tidak tersedia untuk beberapa pengguna</span><span class="sxs-lookup"><span data-stu-id="03133-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="03133-103">SharePoint atau OneDrive mungkin lambat, tidak dapat diakses, atau tidak tersedia, atau mungkin menampilkan kesalahan layanan yang tidak tersedia atau 503, karena beberapa alasan:</span><span class="sxs-lookup"><span data-stu-id="03133-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="03133-104">Jika situs SharePoint atau OneDrive Anda lambat atau tertunda untuk beberapa pengguna, mungkin ada masalah layanan sementara ketika pengguna mengalami keterlambatan atau kesalahan navigasi saat mengakses situs SharePoint atau konten OneDrive.</span><span class="sxs-lookup"><span data-stu-id="03133-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="03133-105">Lihat [dasbor Kesehatan Layanan](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) untuk melihat apakah organisasi Anda terpengaruh.</span><span class="sxs-lookup"><span data-stu-id="03133-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="03133-106">Pengguna mungkin menerima *server 503 adalah kesalahan sibuk* ketika mencoba menavigasi ke situs SharePoint atau OneDrive.</span><span class="sxs-lookup"><span data-stu-id="03133-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="03133-107">Kesalahan ini bisa disebabkan oleh pembatasan dalam Layanan SharePoint.</span><span class="sxs-lookup"><span data-stu-id="03133-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="03133-108">SharePoint Online menerapkan pembatasan untuk mempertahankan kinerja yang optimal dan keandalan layanan SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="03133-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="03133-109">Pembatasan membatasi jumlah tindakan pengguna atau panggilan serentak (berdasarkan skrip atau kode) untuk mencegah penggunaan sumber daya secara berlebihan.</span><span class="sxs-lookup"><span data-stu-id="03133-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="03133-110">Untuk informasi selengkapnya tentang pembatasan, [Hindari mendapatkan pembatasan atau diblokir di SharePoint online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="03133-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="03133-111">Jika Anda mengalami kinerja yang lambat dengan situs atau halaman SharePoint **klasik** atau **modern** , gunakan [alat diagnostik halaman](https://aka.ms/perftool) untuk menganalisis halaman.</span><span class="sxs-lookup"><span data-stu-id="03133-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="03133-112">Jika Anda masih mengalami kinerja yang lambat umum, silakan Tinjau sumber daya di bagian bawah artikel ini: [pengenalan ke tuning kinerja untuk SharePoint online](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="03133-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  