---
title: Tidak dapat menambahkan 2010 persetujuan alur kerja
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: aa61f1615b60d27cffad15f02f6ce5dbac1b607f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47699738"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="24675-102">Tidak dapat menambahkan 2010 persetujuan alur kerja</span><span class="sxs-lookup"><span data-stu-id="24675-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="24675-103">Dalam kumpulan situs Microsoft SharePoint, Anda tidak bisa menambahkan alur kerja yang dapat digunakan kembali secara global (seperti "persetujuan-SharePoint 2010") ke daftar atau pustaka.</span><span class="sxs-lookup"><span data-stu-id="24675-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="24675-104">Untuk mengatasi masalah ini, ikuti langkah-langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="24675-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="24675-105">Buka situs web akar kumpulan situs di SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="24675-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="24675-106">Di bawah **objek situs**, pilih **alur kerja**.</span><span class="sxs-lookup"><span data-stu-id="24675-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="24675-107">Di bagian **baru** pita **alur kerja** , pilih **alur kerja yang dapat digunakan kembali**.</span><span class="sxs-lookup"><span data-stu-id="24675-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="24675-108">Pada formulir **buat alur kerja yang dapat digunakan kembali** , masukkan nama \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="24675-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="24675-109">Untuk **tipe platform**, klik **alur kerja SharePoint 2010**, lalu klik **OK**.</span><span class="sxs-lookup"><span data-stu-id="24675-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="24675-110">Di bagian **Simpan** pada pita **alur kerja** , pilih **terbitkan**.</span><span class="sxs-lookup"><span data-stu-id="24675-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="24675-111">Di bagian **Kelola** dari pita **alur kerja** , pilih **terbitkan secara global**.</span><span class="sxs-lookup"><span data-stu-id="24675-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="24675-112">Dalam kotak dialog konfirmasi yang muncul, pilih **OK**.</span><span class="sxs-lookup"><span data-stu-id="24675-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="24675-113">Di browser web, temukan situs web akar dari kumpulan situs, lalu akses **Site Settings** \> **fitur kumpulan situs**pengaturan situs.</span><span class="sxs-lookup"><span data-stu-id="24675-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="24675-114">Mengaktifkan fitur **alur kerja** :</span><span class="sxs-lookup"><span data-stu-id="24675-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="24675-115">· Jika fitur  *diaktifkan*  , klik **Nonaktifkan,** lalu klik **Aktifkan**.</span><span class="sxs-lookup"><span data-stu-id="24675-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="24675-116">· Jika fitur  *dinonaktifkan*  , klik **Aktifkan**.</span><span class="sxs-lookup"><span data-stu-id="24675-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="24675-117">Untuk informasi selengkapnya, lihat [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)berikut ini.</span><span class="sxs-lookup"><span data-stu-id="24675-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

