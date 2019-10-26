---
title: Alur kerja tidak dimulai
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 2d85dcf9111d48cb529c583c733823b404eb3188
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/25/2019
ms.locfileid: "36738092"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="80cde-102">Alur kerja tidak dimulai</span><span class="sxs-lookup"><span data-stu-id="80cde-102">Workflow is not starting</span></span>

- <span data-ttu-id="80cde-103">SharePoint 2010 dan SharePoint 2013 alur kerja tidak dimulai.</span><span class="sxs-lookup"><span data-stu-id="80cde-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="80cde-104">Jika alur kerja Anda tidak dimulai, mungkin ada masalah layanan sementara di mana pengguna mungkin mengalami penundaan terputus-putus dengan kemajuan alur kerja.</span><span class="sxs-lookup"><span data-stu-id="80cde-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="80cde-105">Periksa [dasbor Kesehatan Layanan](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) untuk melihat apakah organisasi Anda terpengaruh.</span><span class="sxs-lookup"><span data-stu-id="80cde-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="80cde-106">Jika lebih dari 24 jam telah berlalu sejak Anda pertama kali melihat masalah ini, silakan log tiket dukungan.</span><span class="sxs-lookup"><span data-stu-id="80cde-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="80cde-107">Dalam banyak kasus, kami telah bekerja pada solusi.</span><span class="sxs-lookup"><span data-stu-id="80cde-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="80cde-108">Tolong beri kami setidaknya 24 jam untuk menyelesaikan solusi.</span><span class="sxs-lookup"><span data-stu-id="80cde-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="80cde-109">SharePoint 2010 alur kerja tertunda pada mulai.</span><span class="sxs-lookup"><span data-stu-id="80cde-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="80cde-110">Hal ini terjadi jika alur kerja dipicu dalam batch besar.</span><span class="sxs-lookup"><span data-stu-id="80cde-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="80cde-111">(misalnya, ketika beberapa item ditambahkan sekaligus).</span><span class="sxs-lookup"><span data-stu-id="80cde-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="80cde-112">Alur kerja tidak dirancang untuk berjalan secara real-time, sehingga penundaan adalah perilaku dengan desain.</span><span class="sxs-lookup"><span data-stu-id="80cde-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="80cde-113">Jika alur kerja kompleks extensible objek Markup Language (XMOL), kompilasi dapat lambat.</span><span class="sxs-lookup"><span data-stu-id="80cde-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="80cde-114">Periksa artikel [ini](https://support.microsoft.com//kb/3043697) .</span><span class="sxs-lookup"><span data-stu-id="80cde-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="80cde-115">Anda harus menyederhanakan alur kerja atau mendesain ulang menggunakan jenis platform Microsoft SharePoint 2013 alur kerja.</span><span class="sxs-lookup"><span data-stu-id="80cde-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="80cde-116">Jika Riwayat alur kerja Anda tumbuh besar, Anda mungkin ingin membersihkan item atau membuat daftar Riwayat baru.</span><span class="sxs-lookup"><span data-stu-id="80cde-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="80cde-117">Informasi lebih lanjut: [membersihkan riwayat alur kerja](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="80cde-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="80cde-118">Topik terkait</span><span class="sxs-lookup"><span data-stu-id="80cde-118">Related topics</span></span>
<span data-ttu-id="80cde-119">Ingin mencoba Microsoft Flow di SharePoint online?</span><span class="sxs-lookup"><span data-stu-id="80cde-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="80cde-120">Membuat Flow</span><span class="sxs-lookup"><span data-stu-id="80cde-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="80cde-121">SharePoint dan aliran</span><span class="sxs-lookup"><span data-stu-id="80cde-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


