---
title: Alur kerja tidak dimulai
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403746"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="e3576-102">Alur kerja tidak dimulai</span><span class="sxs-lookup"><span data-stu-id="e3576-102">Workflow is not starting</span></span>

- <span data-ttu-id="e3576-103">Alur kerja SharePoint 2010 dan SharePoint 2013 tidak dimulai.</span><span class="sxs-lookup"><span data-stu-id="e3576-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="e3576-104">Jika alur kerja Anda tidak dimulai, mungkin terdapat masalah layanan sementara ketika pengguna mungkin mengalami penundaan sebentar-sebentar dengan kemajuan alur kerja.</span><span class="sxs-lookup"><span data-stu-id="e3576-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="e3576-105">Periksa Dasbor [Kesehatan Layanan untuk](https://admin.microsoft.com/AdminPortal/Home/servicehealth) melihat apakah organisasi Anda terkena dampak.</span><span class="sxs-lookup"><span data-stu-id="e3576-105">Check the [Service Health Dashboard](https://admin.microsoft.com/AdminPortal/Home/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="e3576-106">Jika sudah lebih dari 24 jam sejak masalah ini muncul pertama kali, silakan log tiket dukungan.</span><span class="sxs-lookup"><span data-stu-id="e3576-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="e3576-107">Dalam banyak kasus, kami sedang mencari solusi.</span><span class="sxs-lookup"><span data-stu-id="e3576-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="e3576-108">Harap beri kami setidaknya 24 jam untuk menyelesaikan solusi.</span><span class="sxs-lookup"><span data-stu-id="e3576-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="e3576-109">Alur kerja SharePoint 2010 tertunda saat dimulai.</span><span class="sxs-lookup"><span data-stu-id="e3576-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="e3576-110">Hal ini terjadi jika alur kerja dipicu dalam kumpulan yang besar.</span><span class="sxs-lookup"><span data-stu-id="e3576-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="e3576-111">(misalnya, ketika beberapa item ditambahkan sekaligus).</span><span class="sxs-lookup"><span data-stu-id="e3576-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="e3576-112">Alur kerja tidak dirancang untuk berjalan secara real-time, jadi penundaan adalah perilaku berdasarkan desain.</span><span class="sxs-lookup"><span data-stu-id="e3576-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="e3576-113">Jika Alur Kerja kompleks Extensible Object Markup Language (X HTML), kompilasi bisa lambat.</span><span class="sxs-lookup"><span data-stu-id="e3576-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="e3576-114">Periksa [artikel](https://support.microsoft.com//kb/3043697) ini.</span><span class="sxs-lookup"><span data-stu-id="e3576-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="e3576-115">Anda harus menyederhanakan alur kerja atau mendesain ulang alur kerja menggunakan tipe platform Alur Kerja Microsoft SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="e3576-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="e3576-116">Jika riwayat alur kerja Anda bertambah besar, Anda mungkin ingin membersihkan item atau membuat daftar riwayat baru.</span><span class="sxs-lookup"><span data-stu-id="e3576-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="e3576-117">Informasi Selengkapnya : [Membersihkan riwayat alur kerja](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="e3576-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="e3576-118">Topik terkait</span><span class="sxs-lookup"><span data-stu-id="e3576-118">Related topics</span></span>
<span data-ttu-id="e3576-119">Ingin mencoba Microsoft Flow di SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="e3576-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="e3576-120">Membuat Alur</span><span class="sxs-lookup"><span data-stu-id="e3576-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="e3576-121">SharePoint dan Aliran</span><span class="sxs-lookup"><span data-stu-id="e3576-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
