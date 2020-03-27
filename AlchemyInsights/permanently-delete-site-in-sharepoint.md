---
title: Menghapus situs di SharePoint secara permanen
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: 263317339d965d173a5a038fa006e0ce6f8476cc
ms.sourcegitcommit: da04e79b6072321caa16a6ceea6eb5f15de22394
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 03/25/2020
ms.locfileid: "42955167"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a><span data-ttu-id="77c75-102">Menghapus situs di SharePoint secara permanen</span><span class="sxs-lookup"><span data-stu-id="77c75-102">Permanently delete a site in SharePoint</span></span>

<span data-ttu-id="77c75-103">Untuk menggunakan kembali URL dari situs yang telah dihapus (untuk membuat ulang situs), atau untuk menghapus situs secara permanen karena tidak digunakan lagi, Anda dapat menggunakan opsi **Hapus Secara Permanen** dari Pusat Admin SharePoint baru.</span><span class="sxs-lookup"><span data-stu-id="77c75-103">To reuse a URL from a deleted site (to recreate a site), or to permanently delete a site because it's no longer in use, you can use **Permanently Delete** from the New SharePoint Admin Center.</span></span> 

1. <span data-ttu-id="77c75-104">Buka [halaman situs yang telah dihapus di Pusat admin SharePoint baru](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) lalu masuk dengan akun yang memiliki izin admin untuk organisasi Anda.</span><span class="sxs-lookup"><span data-stu-id="77c75-104">Go to the [Deleted sites page of the new SharePoint admin center](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) and sign in with an account that has admin permissions for your organization.</span></span> 

2. <span data-ttu-id="77c75-105">Di kolom sebelah kiri, pilih sebuah situs.</span><span class="sxs-lookup"><span data-stu-id="77c75-105">In the left column, select a site.</span></span> 

3. <span data-ttu-id="77c75-106">Klik **Hapus Secara Permanen**.</span><span class="sxs-lookup"><span data-stu-id="77c75-106">Click **Permanently Delete**.</span></span> 

<span data-ttu-id="77c75-107">**Catatan**: Situs yang terkait dengan grup tidak dapat dihapus secara permanen dari Pusat Admin SharePoint baru.</span><span class="sxs-lookup"><span data-stu-id="77c75-107">**Note**: Group-connected sites cannot be permanently deleted from the New SharePoint Admin Center.</span></span> <span data-ttu-id="77c75-108">Sebagai gantinya, gunakan [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite).</span><span class="sxs-lookup"><span data-stu-id="77c75-108">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) will need to be used instead.</span></span>  

<span data-ttu-id="77c75-109">Untuk informasi selengkapnya, lihat [Menghapus situs secara permanen](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="77c75-109">For more info, see [Permanently delete a site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span></span> 
