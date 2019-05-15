---
title: Akses layanan pensiun
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 395dac6abf1562aa0da0b1d87eddd943affefc3f
ms.sourcegitcommit: b2c9202b94fa1ce73dbeb3e43b219ba07e46e7e3
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/14/2019
ms.locfileid: "33973926"
---
# <a name="access-services-retirement"></a><span data-ttu-id="af377-102">Akses layanan pensiun</span><span class="sxs-lookup"><span data-stu-id="af377-102">Access services retirement</span></span>

<span data-ttu-id="af377-103">Seperti yang kita awalnya diumumkan di MC97576, pada Maret 2017, dan terus berkomunikasi selama setahun layanan akses yang sedang dihentikan dari Office 365.</span><span class="sxs-lookup"><span data-stu-id="af377-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="af377-104">Tahap berikutnya dalam proses ini akan penghapusan akses Web database yang menggunakan daftar SharePoint sebagai penyimpanan data yang mendasari mereka.</span><span class="sxs-lookup"><span data-stu-id="af377-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

## <a name="how-does-this-affect-me"></a><span data-ttu-id="af377-105">Bagaimana ini mempengaruhi saya?</span><span class="sxs-lookup"><span data-stu-id="af377-105">How does this affect me?</span></span>

<span data-ttu-id="af377-106">Mulai Juni 2019, kami akan berhenti penciptaan baru akses database dalam SharePoint Online dan menutup layanan dan aplikasi sisa 2020 April.</span><span class="sxs-lookup"><span data-stu-id="af377-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

## <a name="what-do-i-need-to-do-to-prepare-for-this-change"></a><span data-ttu-id="af377-107">Apa yang harus saya lakukan untuk mempersiapkan untuk perubahan ini?</span><span class="sxs-lookup"><span data-stu-id="af377-107">What do I need to do to prepare for this change?</span></span>

<span data-ttu-id="af377-108">Kami mendorong Anda untuk membuat rencana transisi untuk organisasi Anda akses web database.</span><span class="sxs-lookup"><span data-stu-id="af377-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="af377-109">Admin dapat menggunakan [scanner aplikasi SharePoint akses](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) untuk memperoleh inventarisasi akses aplikasi yang menggunakan situs.</span><span class="sxs-lookup"><span data-stu-id="af377-109">Admins can use the [SharePoint Access app scanner](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) to obtain an inventory of the Access apps that sites are using.</span></span> 

<span data-ttu-id="af377-110">Ada beberapa cara untuk memigrasi data database Access web:</span><span class="sxs-lookup"><span data-stu-id="af377-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="af377-111">Mengimpor ke database akses lokal (. ACCDB) atau ke Excel file.</span><span class="sxs-lookup"><span data-stu-id="af377-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="af377-112">Kami juga merekomendasikan menjelajahi Microsoft PowerApps sebagai platform alternatif untuk menciptakan solusi bisnis tidak kode untuk web dan perangkat mobile.</span><span class="sxs-lookup"><span data-stu-id="af377-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>