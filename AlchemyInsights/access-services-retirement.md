---
title: Pensiun Layanan Access
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698685"
---
# <a name="access-services-retirement"></a><span data-ttu-id="84f4d-102">Pensiun Layanan Access</span><span class="sxs-lookup"><span data-stu-id="84f4d-102">Access services retirement</span></span>

<span data-ttu-id="84f4d-103">Seperti yang kami Umumkan di MC97576, pada bulan Maret 2017, dan melanjutkan untuk berkomunikasi selama tahun lalu Layanan Access telah dihentikan.</span><span class="sxs-lookup"><span data-stu-id="84f4d-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired.</span></span> <span data-ttu-id="84f4d-104">Fase berikutnya dalam proses ini adalah penghapusan database Web Access yang menggunakan daftar SharePoint sebagai penyimpanan data yang mendasari.</span><span class="sxs-lookup"><span data-stu-id="84f4d-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="84f4d-105">**Bagaimana hal ini mempengaruhi saya?**</span><span class="sxs-lookup"><span data-stu-id="84f4d-105">**How does this affect me?**</span></span>

<span data-ttu-id="84f4d-106">Mulai 2019 Juni, kami akan menghentikan pembuatan database Access baru di SharePoint online dan menutup layanan dan aplikasi yang tersisa pada bulan April 2020.</span><span class="sxs-lookup"><span data-stu-id="84f4d-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="84f4d-107">**Apa yang perlu saya lakukan untuk mempersiapkan perubahan ini?**</span><span class="sxs-lookup"><span data-stu-id="84f4d-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="84f4d-108">Kami menyarankan agar Anda membuat rencana transisi untuk database Web Access organisasi Anda.</span><span class="sxs-lookup"><span data-stu-id="84f4d-108">We encourage you to create a transition plan for your organization's Access web databases.</span></span> <span data-ttu-id="84f4d-109">Admin dapat menggunakan [pemindai aplikasi akses SharePoint](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) untuk mendapatkan inventaris aplikasi Access yang digunakan situs.</span><span class="sxs-lookup"><span data-stu-id="84f4d-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="84f4d-110">Ada beberapa cara untuk melakukan migrasi data database Web Access:</span><span class="sxs-lookup"><span data-stu-id="84f4d-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="84f4d-111">Mengimpor ke database Access lokal (. ACCDB) atau ke file Excel.</span><span class="sxs-lookup"><span data-stu-id="84f4d-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="84f4d-112">Kami juga merekomendasikan menjelajahi Microsoft PowerApps sebagai platform alternatif untuk membuat solusi bisnis tanpa kode untuk perangkat web dan seluler.</span><span class="sxs-lookup"><span data-stu-id="84f4d-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>