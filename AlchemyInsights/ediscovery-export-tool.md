---
title: Alat ekspor eDiscovery
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814591"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="947f9-102">Tidak dapat menginstal atau menjalankan Alat Ekspor eDiscovery?</span><span class="sxs-lookup"><span data-stu-id="947f9-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="947f9-103">Jika tidak dapat menginstal atau menjalankan Alat Ekspor eDiscovery untuk mengunduh hasil pencarian, periksa hal-hal berikut:</span><span class="sxs-lookup"><span data-stu-id="947f9-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="947f9-104">Komputer yang Anda gunakan memenuhi prasyarat berikut:</span><span class="sxs-lookup"><span data-stu-id="947f9-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="947f9-105">Windows 7 versi 32- atau 64-bit dan versi yang lebih baru</span><span class="sxs-lookup"><span data-stu-id="947f9-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="947f9-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="947f9-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="947f9-107">Browser yang didukung:</span><span class="sxs-lookup"><span data-stu-id="947f9-107">A supported browser:</span></span>

  - <span data-ttu-id="947f9-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="947f9-108">Microsoft Edge</span></span>

    <span data-ttu-id="947f9-109">Atau</span><span class="sxs-lookup"><span data-stu-id="947f9-109">Or</span></span>

  - <span data-ttu-id="947f9-110">Internet Explorer 10 dan versi yang lebih baru</span><span class="sxs-lookup"><span data-stu-id="947f9-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="947f9-111">Browser lain, seperti Google Chrome dan Mozilla Firefox tidak didukung.</span><span class="sxs-lookup"><span data-stu-id="947f9-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="947f9-112">Organisasi Anda dapat tersambung ke titik akhir di Azure, yaitu **\* .blob.core.windows.net** (wildcard mewakili pengidentifikasi unik untuk pekerjaan ekspor Anda).</span><span class="sxs-lookup"><span data-stu-id="947f9-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="947f9-113">Anda mendapatkan peran Ekspor di Pusat Kepatuhan Keamanan Microsoft 365. &amp;</span><span class="sxs-lookup"><span data-stu-id="947f9-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="947f9-114">Secara default, peran ini hanya ditetapkan pada grup peran Manajer eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="947f9-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="947f9-115">Lihat [Menetapkan izin eDiscovery.](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)</span><span class="sxs-lookup"><span data-stu-id="947f9-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="947f9-116">Untuk informasi selengkapnya, lihat [Mengekspor hasil Pencarian Konten.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)</span><span class="sxs-lookup"><span data-stu-id="947f9-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="947f9-117">Jika mengekspor lebih dari 100 kotak surat, Anda perlu menggunakan Powershell berikut untuk mengunduh hasil Ekspor: Mengekspor hasil dari lebih dari  [100K](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)kotak surat .</span><span class="sxs-lookup"><span data-stu-id="947f9-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>