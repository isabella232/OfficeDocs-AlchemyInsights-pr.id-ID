---
title: Hilang alur kerja gagal untuk mengaktifkan
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 44fd3c2d1e8b278b47c0fde6d48c7cbcbaa5c324
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36543928"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="3312a-102">Hilang alur kerja gagal untuk mengaktifkan</span><span class="sxs-lookup"><span data-stu-id="3312a-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="3312a-103">Di Microsoft SharePoint situs koleksi, Anda tidak dapat menambahkan alur kerja global dapat digunakan kembali (seperti "persetujuan - SharePoint 2010") ke daftar atau Perpustakaan.</span><span class="sxs-lookup"><span data-stu-id="3312a-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="3312a-104">Untuk mengatasi masalah ini, ikuti langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="3312a-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="3312a-105">Buka situs akar koleksi situs di SharePoint desainer 2013.</span><span class="sxs-lookup"><span data-stu-id="3312a-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="3312a-106">**Benda-benda situs**, pilih **alur kerja**.</span><span class="sxs-lookup"><span data-stu-id="3312a-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="3312a-107">Di bagian **baru** dari pita **alur kerja** , pilih **Reusable alur kerja**.</span><span class="sxs-lookup"><span data-stu-id="3312a-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="3312a-108">Pada bentuk **Membuat Reusable alur kerja** , masukkan nama \*\* *Repair2010* \*\*.</span><span class="sxs-lookup"><span data-stu-id="3312a-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="3312a-109">Untuk **Jenis Platform**, klik **SharePoint 2010 alur kerja**, dan kemudian klik **OK**.</span><span class="sxs-lookup"><span data-stu-id="3312a-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="3312a-110">Di bagian **menyimpan** pita **alur kerja** , pilih **Publish**.</span><span class="sxs-lookup"><span data-stu-id="3312a-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="3312a-111">Di bagian **Manage** pita **alur kerja** , pilih **Mempublikasikan secara global**.</span><span class="sxs-lookup"><span data-stu-id="3312a-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="3312a-112">Di kotak dialog konfirmasi yang muncul, pilih **OK**.</span><span class="sxs-lookup"><span data-stu-id="3312a-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="3312a-113">Di web browser, mencari situs situs koleksi akar, dan mengakses **Pengaturan situs** \> **Situs koleksi fitur**.</span><span class="sxs-lookup"><span data-stu-id="3312a-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="3312a-114">Kemudian, beralih fitur **alur kerja** :</span><span class="sxs-lookup"><span data-stu-id="3312a-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="3312a-115">· Jika fitur *aktif* , klik **Nonaktifkan,** dan kemudian klik **Aktifkan**.</span><span class="sxs-lookup"><span data-stu-id="3312a-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="3312a-116">· Jika fitur *Deactivated* , klik **Aktifkan**.</span><span class="sxs-lookup"><span data-stu-id="3312a-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="3312a-117">Untuk informasi lebih lanjut silakan lihat berikut [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="3312a-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

