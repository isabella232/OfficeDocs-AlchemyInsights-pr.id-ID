---
title: Berbagi dengan pengguna eksternal tidak berfungsi
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: d4c8fc75ff8db2319b88a20bea9b3ee661f2e36e
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/18/2019
ms.locfileid: "36502234"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="e78f3-102">Memperbaiki masalah saat berbagi konten SharePoint dengan pengguna eksternal</span><span class="sxs-lookup"><span data-stu-id="e78f3-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="e78f3-103">Pastikan berbagi eksternal diaktifkan untuk organisasi Anda:</span><span class="sxs-lookup"><span data-stu-id="e78f3-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="e78f3-104">Buka [Halaman Add- &amp; in layanan di pusat admin Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), dan klik **situs**.</span><span class="sxs-lookup"><span data-stu-id="e78f3-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="e78f3-105">Pastikan setelan diubah menjadi "aktif".</span><span class="sxs-lookup"><span data-stu-id="e78f3-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="e78f3-106">Jika "hanya ada pengguna eksternal" dipilih, pastikan pengguna eksternal tercantum di pusat admin Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e78f3-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="e78f3-107">Pastikan berbagi eksternal diaktifkan untuk situs.</span><span class="sxs-lookup"><span data-stu-id="e78f3-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="e78f3-108">Untuk koleksi situs klasik:</span><span class="sxs-lookup"><span data-stu-id="e78f3-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="e78f3-109">Di pusat admin SharePoint baru, di sebelah kiri, klik **situs**.</span><span class="sxs-lookup"><span data-stu-id="e78f3-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="e78f3-110">Pilih situs atau situs, dan pada pita, klik **berbagi**.</span><span class="sxs-lookup"><span data-stu-id="e78f3-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="e78f3-111">Untuk situs tim yang dimiliki oleh grup 365 Office, atau situs komunikasi:</span><span class="sxs-lookup"><span data-stu-id="e78f3-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="e78f3-112">Jenis situs baru ini memiliki setelan berbagi yang sama dengan setelan di seluruh organisasi, kecuali jika setelan di seluruh organisasi memungkinkan berbagi file menggunakan tautan yang tidak memerlukan masuk.</span><span class="sxs-lookup"><span data-stu-id="e78f3-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="e78f3-113">Dalam hal ini, situs memungkinkan berbagi dengan pengguna eksternal baru dan yang ada yang masuk.</span><span class="sxs-lookup"><span data-stu-id="e78f3-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="e78f3-114">Untuk mengubah pengaturan untuk situs tertentu, gunakan Pusat admin SharePoint baru atau PowerShell.</span><span class="sxs-lookup"><span data-stu-id="e78f3-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="e78f3-115">[Pelajari lebih lanjut](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="e78f3-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="e78f3-116">Setelan berbagi eksternal untuk situs mana pun dapat lebih ketat daripada setelan di seluruh organisasi, tetapi tidak lebih permisif daripada setelan di seluruh organisasi.</span><span class="sxs-lookup"><span data-stu-id="e78f3-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

