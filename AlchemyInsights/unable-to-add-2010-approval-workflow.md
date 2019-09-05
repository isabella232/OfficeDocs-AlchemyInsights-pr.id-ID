---
title: Tidak dapat menambahkan 2010 persetujuan alur kerja
ms.author: pebaum
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 13e3ed6db8c31adb1eb5a556c0e5fbc437b3fdb1
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/04/2019
ms.locfileid: "36748687"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="7e90f-102">Tidak dapat menambahkan 2010 persetujuan alur kerja</span><span class="sxs-lookup"><span data-stu-id="7e90f-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="7e90f-103">Dalam koleksi situs Microsoft SharePoint, Anda tidak dapat menambahkan alur kerja global Reusable (seperti "persetujuan-SharePoint 2010") ke daftar atau Perpustakaan.</span><span class="sxs-lookup"><span data-stu-id="7e90f-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="7e90f-104">Untuk mengatasi masalah ini, ikuti langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="7e90f-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="7e90f-105">Buka situs akar koleksi situs di 2013 SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="7e90f-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="7e90f-106">Di bawah **objek situs**, pilih **alur kerja**.</span><span class="sxs-lookup"><span data-stu-id="7e90f-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="7e90f-107">Di bagian **baru** pita **alur kerja** , pilih **alur kerja dapat digunakan kembali**.</span><span class="sxs-lookup"><span data-stu-id="7e90f-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="7e90f-108">Pada formulir **buat alur kerja yang dapat digunakan kembali** , masukkan nama \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="7e90f-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="7e90f-109">Untuk **jenis platform**, klik **alur kerja SharePoint 2010**, dan kemudian klik **OK**.</span><span class="sxs-lookup"><span data-stu-id="7e90f-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="7e90f-110">Di bagian **Simpan** pita **alur kerja** , pilih **terbitkan**.</span><span class="sxs-lookup"><span data-stu-id="7e90f-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="7e90f-111">Di bagian **Kelola** pita **alur kerja** , pilih **terbitkan secara global**.</span><span class="sxs-lookup"><span data-stu-id="7e90f-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="7e90f-112">Di kotak dialog konfirmasi yang muncul, pilih **OK**.</span><span class="sxs-lookup"><span data-stu-id="7e90f-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="7e90f-113">Di web browser, temukan situs akar koleksi situs, dan kemudian akses **situs pengaturan** \> **situs koleksi fitur**.</span><span class="sxs-lookup"><span data-stu-id="7e90f-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="7e90f-114">Beralih fitur **alur kerja** :</span><span class="sxs-lookup"><span data-stu-id="7e90f-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="7e90f-115">· Jika fitur *diaktifkan* , klik **Nonaktifkan,** dan kemudian klik **Aktifkan**.</span><span class="sxs-lookup"><span data-stu-id="7e90f-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="7e90f-116">· Jika fitur *dinonaktifkan* , klik **Aktifkan**.</span><span class="sxs-lookup"><span data-stu-id="7e90f-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="7e90f-117">Untuk informasi lebih lanjut, silakan merujuk ke [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)berikut.</span><span class="sxs-lookup"><span data-stu-id="7e90f-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

