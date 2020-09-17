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
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794770"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="59c01-102">Alur kerja tidak dimulai</span><span class="sxs-lookup"><span data-stu-id="59c01-102">Workflow is not starting</span></span>

- <span data-ttu-id="59c01-103">Alur kerja SharePoint 2010 dan SharePoint 2013 tidak dimulai.</span><span class="sxs-lookup"><span data-stu-id="59c01-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="59c01-104">Jika alur kerja Anda tidak dimulai, mungkin ada masalah layanan sementara ketika pengguna mungkin mengalami penundaan dengan kemajuan alur kerja.</span><span class="sxs-lookup"><span data-stu-id="59c01-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="59c01-105">Lihat [dasbor Kesehatan Layanan](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) untuk melihat apakah organisasi Anda terpengaruh.</span><span class="sxs-lookup"><span data-stu-id="59c01-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="59c01-106">Jika lebih dari 24 jam telah berlalu sejak pertama kali melihat masalah ini, silakan masuk ke tiket dukungan.</span><span class="sxs-lookup"><span data-stu-id="59c01-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="59c01-107">Dalam banyak kasus, kami sedang mengupayakan solusi.</span><span class="sxs-lookup"><span data-stu-id="59c01-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="59c01-108">Harap Beri kami setidaknya 24 jam untuk menyelesaikan solusi.</span><span class="sxs-lookup"><span data-stu-id="59c01-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="59c01-109">Alur kerja SharePoint 2010 tertunda saat mulai.</span><span class="sxs-lookup"><span data-stu-id="59c01-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="59c01-110">Hal ini terjadi jika alur kerja dipicu dalam batch besar.</span><span class="sxs-lookup"><span data-stu-id="59c01-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="59c01-111">(misalnya, ketika beberapa item ditambahkan sekaligus).</span><span class="sxs-lookup"><span data-stu-id="59c01-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="59c01-112">Alur kerja tidak dirancang untuk menjalankan real-time, sehingga penundaan adalah perilaku desain.</span><span class="sxs-lookup"><span data-stu-id="59c01-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="59c01-113">Jika alur kerja kompleks extensible Object Markup Language (XMOL), kompilasi bisa menjadi lambat.</span><span class="sxs-lookup"><span data-stu-id="59c01-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="59c01-114">Lihat artikel [ini](https://support.microsoft.com//kb/3043697) .</span><span class="sxs-lookup"><span data-stu-id="59c01-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="59c01-115">Anda harus menyederhanakan alur kerja atau mendesain ulang menggunakan tipe platform alur kerja Microsoft SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="59c01-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="59c01-116">Jika Riwayat alur kerja Anda telah bertambah besar, Anda mungkin ingin menghapus item atau membuat daftar Riwayat baru.</span><span class="sxs-lookup"><span data-stu-id="59c01-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="59c01-117">Informasi selengkapnya: [membersihkan riwayat alur kerja](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="59c01-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="59c01-118">Topik terkait</span><span class="sxs-lookup"><span data-stu-id="59c01-118">Related topics</span></span>
<span data-ttu-id="59c01-119">Ingin mencoba Microsoft Flow di SharePoint online?</span><span class="sxs-lookup"><span data-stu-id="59c01-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="59c01-120">Buat alur</span><span class="sxs-lookup"><span data-stu-id="59c01-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="59c01-121">SharePoint dan Flow</span><span class="sxs-lookup"><span data-stu-id="59c01-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


