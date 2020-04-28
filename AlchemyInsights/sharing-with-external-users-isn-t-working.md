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
ms.openlocfilehash: 37da77c73b3abbdcf9cb2b9c4c43f31eea3c0a49
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/27/2020
ms.locfileid: "43913005"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="862c4-102">Memperbaiki masalah saat berbagi konten SharePoint dengan pengguna eksternal</span><span class="sxs-lookup"><span data-stu-id="862c4-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="862c4-103">Pastikan berbagi eksternal diaktifkan untuk organisasi Anda:</span><span class="sxs-lookup"><span data-stu-id="862c4-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="862c4-104">Buka [Halaman Add- &amp; in layanan di pusat admin Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), dan klik **situs**.</span><span class="sxs-lookup"><span data-stu-id="862c4-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="862c4-105">Pastikan setelan diubah menjadi "aktif".</span><span class="sxs-lookup"><span data-stu-id="862c4-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="862c4-106">Jika "hanya ada pengguna eksternal" dipilih, pastikan pengguna eksternal tercantum di pusat admin Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="862c4-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="862c4-107">Pastikan berbagi eksternal diaktifkan untuk situs.</span><span class="sxs-lookup"><span data-stu-id="862c4-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="862c4-108">Untuk koleksi situs klasik:</span><span class="sxs-lookup"><span data-stu-id="862c4-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="862c4-109">Di pusat admin SharePoint baru, di sebelah kiri, klik **situs**.</span><span class="sxs-lookup"><span data-stu-id="862c4-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="862c4-110">Pilih situs atau situs, dan pada pita, klik **berbagi**.</span><span class="sxs-lookup"><span data-stu-id="862c4-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="862c4-111">Untuk situs tim yang dimiliki oleh grup 365 Microsoft, atau situs komunikasi:</span><span class="sxs-lookup"><span data-stu-id="862c4-111">For a team site that belongs to an Microsoft 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="862c4-112">Jenis situs baru ini memiliki setelan berbagi yang sama dengan setelan di seluruh organisasi, kecuali jika setelan di seluruh organisasi memungkinkan berbagi file menggunakan tautan yang tidak memerlukan masuk.</span><span class="sxs-lookup"><span data-stu-id="862c4-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="862c4-113">Dalam hal ini, situs memungkinkan berbagi dengan pengguna eksternal baru dan yang ada yang masuk.</span><span class="sxs-lookup"><span data-stu-id="862c4-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="862c4-114">Untuk mengubah pengaturan untuk situs tertentu, gunakan Pusat admin SharePoint baru atau PowerShell.</span><span class="sxs-lookup"><span data-stu-id="862c4-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="862c4-115">[Pelajari selengkapnya](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="862c4-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="862c4-116">Setelan berbagi eksternal untuk situs mana pun dapat lebih ketat daripada setelan di seluruh organisasi, tetapi tidak lebih permisif daripada setelan di seluruh organisasi.</span><span class="sxs-lookup"><span data-stu-id="862c4-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

