---
title: Akses layanan pensiun
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 197366882468ebc87fc26f2fe2733371790d1871
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/25/2019
ms.locfileid: "36747787"
---
# <a name="access-services-retirement"></a><span data-ttu-id="aeb89-102">Akses layanan pensiun</span><span class="sxs-lookup"><span data-stu-id="aeb89-102">Access services retirement</span></span>

<span data-ttu-id="aeb89-103">Seperti yang kita awalnya diumumkan di MC97576, pada Maret 2017, dan terus berkomunikasi selama tahun lalu layanan akses sedang pensiun dari 365 Office.</span><span class="sxs-lookup"><span data-stu-id="aeb89-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="aeb89-104">Tahap berikutnya dalam proses ini akan penghapusan akses web database yang menggunakan daftar SharePoint sebagai penyimpanan data dasar mereka.</span><span class="sxs-lookup"><span data-stu-id="aeb89-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="aeb89-105">**Bagaimana hal ini mempengaruhi saya?**</span><span class="sxs-lookup"><span data-stu-id="aeb89-105">**How does this affect me?**</span></span>

<span data-ttu-id="aeb89-106">Mulai 2019 Juni, kami akan menghentikan pembuatan database Access baru di SharePoint online dan menutup layanan dan aplikasi yang tersisa dengan 2020 April.</span><span class="sxs-lookup"><span data-stu-id="aeb89-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="aeb89-107">**Apa yang harus saya lakukan untuk mempersiapkan perubahan ini?**</span><span class="sxs-lookup"><span data-stu-id="aeb89-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="aeb89-108">Kami mendorong Anda untuk membuat rencana transisi untuk database web akses organisasi Anda.</span><span class="sxs-lookup"><span data-stu-id="aeb89-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="aeb89-109">Admin dapat menggunakan [pemindai aplikasi SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) untuk mendapatkan inventaris aplikasi Access yang menggunakan situs.</span><span class="sxs-lookup"><span data-stu-id="aeb89-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="aeb89-110">Ada beberapa cara untuk bermigrasi akses data web database:</span><span class="sxs-lookup"><span data-stu-id="aeb89-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="aeb89-111">Mengimpor ke pangkalan data akses lokal (. ACCDB) atau ke file Excel.</span><span class="sxs-lookup"><span data-stu-id="aeb89-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="aeb89-112">Kami juga menyarankan untuk menjelajahi Microsoft PowerApps sebagai platform alternatif untuk membuat solusi bisnis tanpa kode untuk perangkat seluler dan web.</span><span class="sxs-lookup"><span data-stu-id="aeb89-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>