---
title: Alur kerja tidak memulai
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
ms.openlocfilehash: a3bac74c19a77b7703f948c1d8b6bcd182e9b075
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270783"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="14104-102">Alur kerja tidak memulai</span><span class="sxs-lookup"><span data-stu-id="14104-102">Workflow is not starting</span></span>

- <span data-ttu-id="14104-103">SharePoint 2010 dan SharePoint 2013 alur kerja tidak mulai.</span><span class="sxs-lookup"><span data-stu-id="14104-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="14104-104">Jika alur kerja Anda tidak memulai, mungkin ada masalah sementara layanan mana pengguna mungkin mengalami penundaan intermiten dengan kemajuan alur kerja.</span><span class="sxs-lookup"><span data-stu-id="14104-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="14104-105">Periksa [Layanan kesehatan Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) untuk melihat jika organisasi Anda dipengaruhi.</span><span class="sxs-lookup"><span data-stu-id="14104-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="14104-106">Jika lebih dari 24 jam telah berlalu sejak Anda pertama kali melihat masalah ini, silakan log tiket support.</span><span class="sxs-lookup"><span data-stu-id="14104-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="14104-107">Dalam banyak kasus, kami sudah bekerja pada sebuah solusi.</span><span class="sxs-lookup"><span data-stu-id="14104-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="14104-108">Mohon berikan setidaknya 24 jam untuk menyelesaikan solusi.</span><span class="sxs-lookup"><span data-stu-id="14104-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="14104-109">SharePoint 2010 Workflow tertunda pada awal.</span><span class="sxs-lookup"><span data-stu-id="14104-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="14104-110">Hal ini terjadi jika alur kerja dipicu dalam kumpulan besar.</span><span class="sxs-lookup"><span data-stu-id="14104-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="14104-111">(sebagai contoh, ketika beberapa item ditambahkan sekaligus).</span><span class="sxs-lookup"><span data-stu-id="14104-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="14104-112">Alur kerja tidak dirancang untuk menjalankan real-time, sehingga penundaan adalah perilaku oleh desain.</span><span class="sxs-lookup"><span data-stu-id="14104-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="14104-113">Jika alur kerja adalah kompleks Extensible Object Markup Language (XMOL), kompilasi bisa lambat.</span><span class="sxs-lookup"><span data-stu-id="14104-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="14104-114">Check [this](https://support.microsoft.com/en-us/kb/3043697) artikel.</span><span class="sxs-lookup"><span data-stu-id="14104-114">Check [this](https://support.microsoft.com/en-us/kb/3043697) article.</span></span>

    - <span data-ttu-id="14104-115">Anda harus menyederhanakan alur kerja atau mendesain ulang menggunakan jenis platform Microsoft SharePoint 2013 alur kerja.</span><span class="sxs-lookup"><span data-stu-id="14104-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="14104-116">Jika Riwayat alur kerja telah tumbuh besar, Anda mungkin ingin membersihkan item atau membuat daftar sejarah baru.</span><span class="sxs-lookup"><span data-stu-id="14104-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="14104-117">Informasi lebih lanjut: [membersihkan riwayat alur kerja](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="14104-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="14104-118">Topik terkait</span><span class="sxs-lookup"><span data-stu-id="14104-118">Related topics</span></span>
<span data-ttu-id="14104-119">Ingin mencoba Microsoft Flow di SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="14104-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="14104-120">Menciptakan aliran</span><span class="sxs-lookup"><span data-stu-id="14104-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="14104-121">SharePoint dan aliran</span><span class="sxs-lookup"><span data-stu-id="14104-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 

