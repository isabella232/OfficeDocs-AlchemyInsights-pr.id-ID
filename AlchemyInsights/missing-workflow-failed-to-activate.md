---
title: Alur kerja hilang gagal Aktifkan
ms.author: pebaum
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: f03d7e1441465050c4b0608f4100f217b183d2e2
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 11/15/2019
ms.locfileid: "36753799"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="d1bbb-102">Alur kerja hilang gagal Aktifkan</span><span class="sxs-lookup"><span data-stu-id="d1bbb-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="d1bbb-103">Dalam koleksi situs Microsoft SharePoint, Anda tidak dapat menambahkan alur kerja global Reusable (seperti "persetujuan-SharePoint 2010") ke daftar atau Perpustakaan.</span><span class="sxs-lookup"><span data-stu-id="d1bbb-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="d1bbb-104">Untuk mengatasi masalah ini, ikuti langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="d1bbb-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="d1bbb-105">Buka situs akar koleksi situs di 2013 SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="d1bbb-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="d1bbb-106">Di bawah **objek situs**, pilih **alur kerja**.</span><span class="sxs-lookup"><span data-stu-id="d1bbb-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="d1bbb-107">Di bagian **baru** pita **alur kerja** , pilih **alur kerja dapat digunakan kembali**.</span><span class="sxs-lookup"><span data-stu-id="d1bbb-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="d1bbb-108">Pada formulir **buat alur kerja yang dapat digunakan kembali** , masukkan nama \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="d1bbb-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="d1bbb-109">Untuk **jenis platform**, klik **alur kerja SharePoint 2010**, dan kemudian klik **OK**.</span><span class="sxs-lookup"><span data-stu-id="d1bbb-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="d1bbb-110">Di bagian **Simpan** pita **alur kerja** , pilih **terbitkan**.</span><span class="sxs-lookup"><span data-stu-id="d1bbb-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="d1bbb-111">Di bagian **Kelola** pita **alur kerja** , pilih **terbitkan secara global**.</span><span class="sxs-lookup"><span data-stu-id="d1bbb-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="d1bbb-112">Di kotak dialog konfirmasi yang muncul, pilih **OK**.</span><span class="sxs-lookup"><span data-stu-id="d1bbb-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="d1bbb-113">Di web browser, temukan situs akar koleksi situs, dan kemudian akses **situs pengaturan** \> **situs koleksi fitur**.</span><span class="sxs-lookup"><span data-stu-id="d1bbb-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="d1bbb-114">Kemudian, beralih fitur **alur kerja** :</span><span class="sxs-lookup"><span data-stu-id="d1bbb-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="d1bbb-115">· Jika fitur *diaktifkan* , klik **Nonaktifkan,** dan kemudian klik **Aktifkan**.</span><span class="sxs-lookup"><span data-stu-id="d1bbb-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="d1bbb-116">· Jika fitur *dinonaktifkan* , klik **Aktifkan**.</span><span class="sxs-lookup"><span data-stu-id="d1bbb-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="d1bbb-117">Untuk informasi lebih lanjut, silakan merujuk ke [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)berikut.</span><span class="sxs-lookup"><span data-stu-id="d1bbb-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

