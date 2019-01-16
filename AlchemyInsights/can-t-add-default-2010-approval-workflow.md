---
title: Tidak dapat menambahkan default penyetelan 2010
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2060c9a1-e714-4d93-925e-629c82c35986
ms.openlocfilehash: 758b0339b842478f9609eb716b5b4ddab6579c80
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/15/2019
ms.locfileid: "28294417"
---
# <a name="cant-add-default-2010-approval-workflow"></a><span data-ttu-id="55371-102">Tidak dapat menambahkan default penyetelan 2010</span><span class="sxs-lookup"><span data-stu-id="55371-102">Can't add default 2010 Approval Workflow</span></span>

<span data-ttu-id="55371-103">Di Microsoft SharePoint situs koleksi, Anda tidak dapat menambahkan alur kerja global dapat digunakan kembali (seperti "persetujuan - SharePoint 2010") ke daftar atau Perpustakaan.</span><span class="sxs-lookup"><span data-stu-id="55371-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="55371-104">Untuk mengatasi masalah ini, ikuti langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="55371-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="55371-105">Buka situs akar koleksi situs di SharePoint desainer 2013.</span><span class="sxs-lookup"><span data-stu-id="55371-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="55371-106">**Benda-benda situs**, pilih **alur kerja**.</span><span class="sxs-lookup"><span data-stu-id="55371-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="55371-107">Di bagian **baru** dari pita **alur kerja** , pilih **Reusable alur kerja**.</span><span class="sxs-lookup"><span data-stu-id="55371-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="55371-p101">Pada bentuk **Membuat Reusable alur kerja** , masukkan nama \* \*\*Repair2010\*\*\*. Untuk **Jenis Platform**, pilih **SharePoint 2010 alur kerja**, dan kemudian pilih **OK**.</span><span class="sxs-lookup"><span data-stu-id="55371-p101">On the **Create Reusable Workflow** form, enter the name  \* **Repair2010**\* . For **Platform Type**, select **SharePoint 2010 Workflow**, and then select **OK**.</span></span> 
  
5. <span data-ttu-id="55371-110">Di bagian **menyimpan** pita **alur kerja** , pilih **Publish**.</span><span class="sxs-lookup"><span data-stu-id="55371-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
6. <span data-ttu-id="55371-p102">Di bagian **Manage** pita **alur kerja** , pilih **Mempublikasikan secara global**. Di kotak dialog konfirmasi yang muncul, pilih **OK**.</span><span class="sxs-lookup"><span data-stu-id="55371-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
7. <span data-ttu-id="55371-p103">Di web browser, mencari situs situs koleksi akar, dan mengakses **Pengaturan situs** \> **Situs koleksi fitur**. Kemudian, beralih fitur **alur kerja** :</span><span class="sxs-lookup"><span data-stu-id="55371-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="55371-115">· Jika fitur *aktif* , klik **Nonaktifkan,** dan kemudian klik **Aktifkan**.</span><span class="sxs-lookup"><span data-stu-id="55371-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="55371-116">· Jika fitur *Deactivated* , klik **Aktifkan**.</span><span class="sxs-lookup"><span data-stu-id="55371-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="55371-117">Untuk informasi lebih lanjut silakan lihat berikut [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="55371-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

