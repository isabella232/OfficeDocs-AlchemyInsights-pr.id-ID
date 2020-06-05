---
title: Berbagi dengan pengguna eksternal tidak berfungsi
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 9a40f52637bc8aa7894754118f0f862aa6c71fe2
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582778"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="9694d-102">Memperbaiki masalah saat berbagi konten SharePoint dengan pengguna eksternal</span><span class="sxs-lookup"><span data-stu-id="9694d-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="9694d-103">Pastikan berbagi eksternal diaktifkan untuk organisasi Anda:</span><span class="sxs-lookup"><span data-stu-id="9694d-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="9694d-104">Buka [ &amp; Halaman Add-in layanan di pusat admin Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), dan klik **situs**.</span><span class="sxs-lookup"><span data-stu-id="9694d-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="9694d-105">Pastikan setelan diubah menjadi "aktif".</span><span class="sxs-lookup"><span data-stu-id="9694d-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="9694d-106">Jika "hanya ada pengguna eksternal" dipilih, pastikan pengguna eksternal tercantum di pusat admin Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="9694d-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="9694d-107">Pastikan berbagi eksternal diaktifkan untuk situs.</span><span class="sxs-lookup"><span data-stu-id="9694d-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="9694d-108">Untuk koleksi situs klasik:</span><span class="sxs-lookup"><span data-stu-id="9694d-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="9694d-109">Di pusat admin SharePoint baru, di sebelah kiri, klik **situs**.</span><span class="sxs-lookup"><span data-stu-id="9694d-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="9694d-110">Pilih situs atau situs, dan pada pita, klik **berbagi**.</span><span class="sxs-lookup"><span data-stu-id="9694d-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="9694d-111">Untuk situs tim milik Grup 365 Microsoft, atau situs komunikasi:</span><span class="sxs-lookup"><span data-stu-id="9694d-111">For a team site that belongs to a Microsoft 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="9694d-112">Jenis situs baru ini memiliki setelan berbagi yang sama dengan setelan di seluruh organisasi, kecuali jika setelan di seluruh organisasi memungkinkan berbagi file menggunakan tautan yang tidak memerlukan masuk.</span><span class="sxs-lookup"><span data-stu-id="9694d-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="9694d-113">Dalam hal ini, situs memungkinkan berbagi dengan pengguna eksternal baru dan yang ada yang masuk.</span><span class="sxs-lookup"><span data-stu-id="9694d-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="9694d-114">Untuk mengubah pengaturan untuk situs tertentu, gunakan Pusat admin SharePoint baru atau PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9694d-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="9694d-115">[Pelajari selengkapnya](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="9694d-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="9694d-116">Setelan berbagi eksternal untuk situs mana pun dapat lebih ketat daripada setelan di seluruh organisasi, tetapi tidak lebih permisif daripada setelan di seluruh organisasi.</span><span class="sxs-lookup"><span data-stu-id="9694d-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

