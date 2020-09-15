---
title: Alur kerja hilang gagal diaktifkan
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 604dc770c5c14ded6a8de1cec9e311b03b69f094
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667089"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="364cb-102">Alur kerja hilang gagal diaktifkan</span><span class="sxs-lookup"><span data-stu-id="364cb-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="364cb-103">Dalam kumpulan situs Microsoft SharePoint, Anda tidak bisa menambahkan alur kerja yang dapat digunakan kembali secara global (seperti "persetujuan-SharePoint 2010") ke daftar atau pustaka.</span><span class="sxs-lookup"><span data-stu-id="364cb-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="364cb-104">Untuk mengatasi masalah ini, ikuti langkah-langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="364cb-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="364cb-105">Buka situs web akar kumpulan situs di SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="364cb-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="364cb-106">Di bawah **objek situs**, pilih **alur kerja**.</span><span class="sxs-lookup"><span data-stu-id="364cb-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="364cb-107">Di bagian **baru** pita **alur kerja** , pilih **alur kerja yang dapat digunakan kembali**.</span><span class="sxs-lookup"><span data-stu-id="364cb-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="364cb-108">Pada formulir **buat alur kerja yang dapat digunakan kembali** , masukkan nama \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="364cb-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="364cb-109">Untuk **tipe platform**, klik **alur kerja SharePoint 2010**, lalu klik **OK**.</span><span class="sxs-lookup"><span data-stu-id="364cb-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="364cb-110">Di bagian **Simpan** pada pita **alur kerja** , pilih **terbitkan**.</span><span class="sxs-lookup"><span data-stu-id="364cb-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="364cb-111">Di bagian **Kelola** dari pita **alur kerja** , pilih **terbitkan secara global**.</span><span class="sxs-lookup"><span data-stu-id="364cb-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="364cb-112">Dalam kotak dialog konfirmasi yang muncul, pilih **OK**.</span><span class="sxs-lookup"><span data-stu-id="364cb-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="364cb-113">Di browser web, temukan situs web akar dari kumpulan situs, lalu akses **Site Settings** \> **fitur kumpulan situs**pengaturan situs.</span><span class="sxs-lookup"><span data-stu-id="364cb-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="364cb-114">Lalu, alihkan fitur **alur kerja** :</span><span class="sxs-lookup"><span data-stu-id="364cb-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="364cb-115">· Jika fitur  *diaktifkan*  , klik **Nonaktifkan,** lalu klik **Aktifkan**.</span><span class="sxs-lookup"><span data-stu-id="364cb-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="364cb-116">· Jika fitur  *dinonaktifkan*  , klik **Aktifkan**.</span><span class="sxs-lookup"><span data-stu-id="364cb-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="364cb-117">Untuk informasi selengkapnya, lihat [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)berikut ini.</span><span class="sxs-lookup"><span data-stu-id="364cb-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

