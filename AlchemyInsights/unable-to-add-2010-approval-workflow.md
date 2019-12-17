---
title: Tidak dapat menambahkan 2010 persetujuan alur kerja
ms.author: pebaum
author: pebaum
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 11ba9bf04f826b0d7465a9a81a36c327e79f4d13
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049556"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="f76e9-102">Tidak dapat menambahkan 2010 persetujuan alur kerja</span><span class="sxs-lookup"><span data-stu-id="f76e9-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="f76e9-103">Dalam koleksi situs Microsoft SharePoint, Anda tidak dapat menambahkan alur kerja global Reusable (seperti "persetujuan-SharePoint 2010") ke daftar atau Perpustakaan.</span><span class="sxs-lookup"><span data-stu-id="f76e9-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="f76e9-104">Untuk mengatasi masalah ini, ikuti langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="f76e9-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="f76e9-105">Buka situs akar koleksi situs di 2013 SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="f76e9-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="f76e9-106">Di bawah **objek situs**, pilih **alur kerja**.</span><span class="sxs-lookup"><span data-stu-id="f76e9-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="f76e9-107">Di bagian **baru** pita **alur kerja** , pilih **alur kerja dapat digunakan kembali**.</span><span class="sxs-lookup"><span data-stu-id="f76e9-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="f76e9-108">Pada formulir **buat alur kerja yang dapat digunakan kembali** , masukkan nama \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="f76e9-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="f76e9-109">Untuk **jenis platform**, klik **alur kerja SharePoint 2010**, dan kemudian klik **OK**.</span><span class="sxs-lookup"><span data-stu-id="f76e9-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="f76e9-110">Di bagian **Simpan** pita **alur kerja** , pilih **terbitkan**.</span><span class="sxs-lookup"><span data-stu-id="f76e9-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="f76e9-111">Di bagian **Kelola** pita **alur kerja** , pilih **terbitkan secara global**.</span><span class="sxs-lookup"><span data-stu-id="f76e9-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="f76e9-112">Di kotak dialog konfirmasi yang muncul, pilih **OK**.</span><span class="sxs-lookup"><span data-stu-id="f76e9-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="f76e9-113">Di web browser, temukan situs akar koleksi situs, dan kemudian akses **situs pengaturan** \> **situs koleksi fitur**.</span><span class="sxs-lookup"><span data-stu-id="f76e9-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="f76e9-114">Beralih fitur **alur kerja** :</span><span class="sxs-lookup"><span data-stu-id="f76e9-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="f76e9-115">· Jika fitur *diaktifkan* , klik **Nonaktifkan,** dan kemudian klik **Aktifkan**.</span><span class="sxs-lookup"><span data-stu-id="f76e9-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="f76e9-116">· Jika fitur *dinonaktifkan* , klik **Aktifkan**.</span><span class="sxs-lookup"><span data-stu-id="f76e9-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="f76e9-117">Untuk informasi lebih lanjut, silakan merujuk ke [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)berikut.</span><span class="sxs-lookup"><span data-stu-id="f76e9-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

