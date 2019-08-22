---
title: Berbagi dengan pengguna eksternal tidak bekerja
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36502234"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="64164-102">Memperbaiki masalah yang berbagi konten SharePoint dengan pengguna eksternal</span><span class="sxs-lookup"><span data-stu-id="64164-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="64164-103">Pastikan eksternal berbagi dihidupkan untuk organisasi Anda:</span><span class="sxs-lookup"><span data-stu-id="64164-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="64164-104">Pergi ke [Layanan &amp; halaman add-in di Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), dan klik **situs**.</span><span class="sxs-lookup"><span data-stu-id="64164-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="64164-105">Pastikan pengaturan diaktifkan "On."</span><span class="sxs-lookup"><span data-stu-id="64164-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="64164-106">Jika "Hanya pengguna eksternal yang ada" dipilih, pastikan pengguna eksternal terdaftar di Microsoft 365 admin center.</span><span class="sxs-lookup"><span data-stu-id="64164-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="64164-107">Pastikan eksternal berbagi dihidupkan untuk situs.</span><span class="sxs-lookup"><span data-stu-id="64164-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="64164-108">Untuk koleksi klasik situs:</span><span class="sxs-lookup"><span data-stu-id="64164-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="64164-109">Di SharePoint admin center baru, dalam pane kiri, klik **situs**.</span><span class="sxs-lookup"><span data-stu-id="64164-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="64164-110">Pilih situs atau situs, dan pada pita, klik **berbagi**.</span><span class="sxs-lookup"><span data-stu-id="64164-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="64164-111">Untuk situs tim milik Grup Office 365, atau situs komunikasi:</span><span class="sxs-lookup"><span data-stu-id="64164-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="64164-112">Jenis situs ini baru memiliki pengaturan berbagi sama sebagai pengaturan seluruh organisasi Anda, kecuali jika pengaturan di seluruh organisasi yang memungkinkan berbagi file menggunakan link yang tidak memerlukan masuk.</span><span class="sxs-lookup"><span data-stu-id="64164-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="64164-113">Dalam kasus ini, situs yang memungkinkan berbagi dengan baru dan yang ada pengguna eksternal yang masuk.</span><span class="sxs-lookup"><span data-stu-id="64164-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="64164-114">Untuk mengubah pengaturan untuk situs tertentu, gunakan baru SharePoint admin center atau PowerShell.</span><span class="sxs-lookup"><span data-stu-id="64164-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="64164-115">[Selengkapnya](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="64164-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="64164-116">Pengaturan berbagi eksternal untuk setiap situs dapat lebih ketat daripada pengaturan seluruh organisasi Anda, tetapi tidak lebih permisif dari pengaturan di seluruh organisasi.</span><span class="sxs-lookup"><span data-stu-id="64164-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

