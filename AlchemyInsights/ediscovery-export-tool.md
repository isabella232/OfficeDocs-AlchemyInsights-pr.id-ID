---
title: Alat ekspor eDiscovery
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277930"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="4295a-102">Tidak dapat menginstal atau menjalankan alat ekspor eDiscovery?</span><span class="sxs-lookup"><span data-stu-id="4295a-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="4295a-103">Jika Anda tidak dapat menginstal atau menjalankan alat ekspor eDiscovery untuk mengunduh hasil pencarian, periksa hal-hal berikut ini:</span><span class="sxs-lookup"><span data-stu-id="4295a-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="4295a-104">Komputer yang Anda gunakan memenuhi prasyarat ini:</span><span class="sxs-lookup"><span data-stu-id="4295a-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="4295a-105">32-atau 64-bit versi Windows 7 dan versi yang lebih baru</span><span class="sxs-lookup"><span data-stu-id="4295a-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="4295a-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="4295a-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="4295a-107">Browser yang didukung:</span><span class="sxs-lookup"><span data-stu-id="4295a-107">A supported browser:</span></span>

  - <span data-ttu-id="4295a-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="4295a-108">Microsoft Edge</span></span>

    <span data-ttu-id="4295a-109">Atau</span><span class="sxs-lookup"><span data-stu-id="4295a-109">Or</span></span>

  - <span data-ttu-id="4295a-110">Internet Explorer 10 dan versi yang lebih baru</span><span class="sxs-lookup"><span data-stu-id="4295a-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="4295a-111">Browser lain, seperti Google Chrome dan Mozilla Firefox tidak didukung.</span><span class="sxs-lookup"><span data-stu-id="4295a-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="4295a-112">Organisasi Anda dapat menyambungkan ke titik akhir di Azure, yaitu \*\* \* . Blob.Core.Windows.net\*\* (wildcard mewakili pengidentifikasi unik untuk pekerjaan ekspor Anda).</span><span class="sxs-lookup"><span data-stu-id="4295a-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="4295a-113">Anda diberi peran ekspor di pusat kepatuhan keamanan Microsoft 365 &amp; .</span><span class="sxs-lookup"><span data-stu-id="4295a-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="4295a-114">Secara default, peran ini hanya ditetapkan ke grup peran Manajer eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="4295a-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="4295a-115">Lihat [menetapkan izin eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span><span class="sxs-lookup"><span data-stu-id="4295a-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="4295a-116">Untuk informasi selengkapnya, lihat [mengekspor hasil pencarian konten](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span><span class="sxs-lookup"><span data-stu-id="4295a-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="4295a-117">Jika Anda mengekspor lebih dari 100K kotak surat, Anda perlu menggunakan PowerShell berikut untuk mengunduh hasil ekspor:  [mengekspor hasil dari kotak surat lebih dari 100k](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="4295a-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>