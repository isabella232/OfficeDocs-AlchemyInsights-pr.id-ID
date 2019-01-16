---
title: Dapat menambahkan penyetelan 2010
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: a83a9621ca0f7764d3f2c0a698dbffd80d55e80c
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/15/2019
ms.locfileid: "28295662"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="89451-102">Dapat menambahkan penyetelan 2010</span><span class="sxs-lookup"><span data-stu-id="89451-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="89451-103">Di Microsoft SharePoint situs koleksi, Anda tidak dapat menambahkan alur kerja global dapat digunakan kembali (seperti "persetujuan - SharePoint 2010") ke daftar atau Perpustakaan.</span><span class="sxs-lookup"><span data-stu-id="89451-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="89451-104">Untuk mengatasi masalah ini, ikuti langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="89451-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="89451-105">Buka situs akar koleksi situs di SharePoint desainer 2013.</span><span class="sxs-lookup"><span data-stu-id="89451-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="89451-106">**Benda-benda situs**, pilih **alur kerja**.</span><span class="sxs-lookup"><span data-stu-id="89451-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="89451-107">Di bagian **baru** dari pita **alur kerja** , pilih **Reusable alur kerja**.</span><span class="sxs-lookup"><span data-stu-id="89451-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="89451-p101">Pada bentuk **Membuat Reusable alur kerja** , masukkan nama \*\* *Repair2010* \*\*. Untuk **Jenis Platform**, klik **SharePoint 2010 alur kerja**, dan kemudian klik **OK**.</span><span class="sxs-lookup"><span data-stu-id="89451-p101">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*. For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="89451-110">Di bagian **menyimpan** pita **alur kerja** , pilih **Publish**.</span><span class="sxs-lookup"><span data-stu-id="89451-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="89451-p102">Di bagian **Manage** pita **alur kerja** , pilih **Mempublikasikan secara global**. Di kotak dialog konfirmasi yang muncul, pilih **OK**.</span><span class="sxs-lookup"><span data-stu-id="89451-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="89451-p103">Di web browser, mencari situs situs koleksi akar, dan mengakses **Pengaturan situs** \> **Situs koleksi fitur**. Beralih fitur **alur kerja** :</span><span class="sxs-lookup"><span data-stu-id="89451-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="89451-115">· Jika fitur *aktif* , klik **Nonaktifkan,** dan kemudian klik **Aktifkan**.</span><span class="sxs-lookup"><span data-stu-id="89451-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="89451-116">· Jika fitur *Deactivated* , klik **Aktifkan**.</span><span class="sxs-lookup"><span data-stu-id="89451-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="89451-117">Untuk informasi lebih lanjut silakan lihat berikut [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="89451-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

