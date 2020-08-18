---
title: Membuat situs SharePoint
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: ba682f3c2b2600031f6856621691b1e0fba64113
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786568"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="f62ed-102">Membuat situs SharePoint</span><span class="sxs-lookup"><span data-stu-id="f62ed-102">Create a SharePoint site</span></span>

<span data-ttu-id="f62ed-103">Membuat atau mengelola situs dari [situs aktif](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) di pusat admin SharePoint.</span><span class="sxs-lookup"><span data-stu-id="f62ed-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="f62ed-104">Untuk informasi selengkapnya, lihat [mengelola situs di pusat admin SharePoint yang baru](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="f62ed-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="f62ed-105">Pipet</span><span class="sxs-lookup"><span data-stu-id="f62ed-105">Tips:</span></span>

- <span data-ttu-id="f62ed-106">Anda **tidak bisa** membuat situs dengan URL yang sama dari situs yang sudah ada.</span><span class="sxs-lookup"><span data-stu-id="f62ed-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="f62ed-107">Jika Anda menghapus situs dan ingin menggunakan kembali URL, mungkin situs yang dihapus masih ada di bawah [situs yang dihapus](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span><span class="sxs-lookup"><span data-stu-id="f62ed-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="f62ed-108">Situs harus dihapus secara permanen untuk menggunakan kembali URL.</span><span class="sxs-lookup"><span data-stu-id="f62ed-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="f62ed-109">Untuk menghapus situs dengan PowerShell, lihat contoh cmdlet [Remove-spsitus](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="f62ed-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="f62ed-110">Beberapa pengguna mungkin tidak bisa membuat situs.</span><span class="sxs-lookup"><span data-stu-id="f62ed-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="f62ed-111">[Lihat mengelola pembuatan situs di SharePoint online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="f62ed-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="f62ed-112">Kemungkinan situs tersebut tampak macet saat **membuat** yang lebih lama dari yang diharapkan.</span><span class="sxs-lookup"><span data-stu-id="f62ed-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="f62ed-113">Jika lebih dari 24 jam telah berlalu sejak pertama kali melihat masalah ini, silakan masuk ke tiket dukungan.</span><span class="sxs-lookup"><span data-stu-id="f62ed-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="f62ed-114">Dalam banyak kasus, kami sedang mengupayakan solusi.</span><span class="sxs-lookup"><span data-stu-id="f62ed-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="f62ed-115">Harap Beri kami setidaknya 24 jam untuk menyelesaikan solusi.</span><span class="sxs-lookup"><span data-stu-id="f62ed-115">Please give us at least 24 hours to complete a solution.</span></span>
