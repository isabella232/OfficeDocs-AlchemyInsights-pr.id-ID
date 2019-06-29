---
title: Akses layanan pensiun
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 5f171050479f34077f3dc155bec40437f86b84c0
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/28/2019
ms.locfileid: "35359352"
---
# <a name="access-services-retirement"></a><span data-ttu-id="20e15-102">Akses layanan pensiun</span><span class="sxs-lookup"><span data-stu-id="20e15-102">Access services retirement</span></span>

<span data-ttu-id="20e15-103">Seperti yang kita awalnya diumumkan di MC97576, pada Maret 2017, dan terus berkomunikasi selama setahun layanan akses yang sedang dihentikan dari Office 365.</span><span class="sxs-lookup"><span data-stu-id="20e15-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="20e15-104">Tahap berikutnya dalam proses ini akan penghapusan akses Web database yang menggunakan daftar SharePoint sebagai penyimpanan data yang mendasari mereka.</span><span class="sxs-lookup"><span data-stu-id="20e15-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="20e15-105">**Bagaimana ini mempengaruhi saya?**</span><span class="sxs-lookup"><span data-stu-id="20e15-105">**How does this affect me?**</span></span>

<span data-ttu-id="20e15-106">Mulai Juni 2019, kami akan berhenti penciptaan baru akses database dalam SharePoint Online dan menutup layanan dan aplikasi sisa 2020 April.</span><span class="sxs-lookup"><span data-stu-id="20e15-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="20e15-107">**Apa yang harus saya lakukan untuk mempersiapkan untuk perubahan ini?**</span><span class="sxs-lookup"><span data-stu-id="20e15-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="20e15-108">Kami mendorong Anda untuk membuat rencana transisi untuk organisasi Anda akses web database.</span><span class="sxs-lookup"><span data-stu-id="20e15-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="20e15-109">Admin dapat menggunakan [scanner aplikasi SharePoint akses](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) untuk memperoleh inventarisasi akses aplikasi yang menggunakan situs.</span><span class="sxs-lookup"><span data-stu-id="20e15-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="20e15-110">Ada beberapa cara untuk memigrasi data database Access web:</span><span class="sxs-lookup"><span data-stu-id="20e15-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="20e15-111">Mengimpor ke database akses lokal (. ACCDB) atau ke Excel file.</span><span class="sxs-lookup"><span data-stu-id="20e15-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="20e15-112">Kami juga merekomendasikan menjelajahi Microsoft PowerApps sebagai platform alternatif untuk menciptakan solusi bisnis tidak kode untuk web dan perangkat mobile.</span><span class="sxs-lookup"><span data-stu-id="20e15-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>