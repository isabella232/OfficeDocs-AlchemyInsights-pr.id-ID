---
title: Membuat situs SharePoint
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 5ebaa342ca9864bc31a9ef26eebcf42d96523871
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806942"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="a73aa-102">Membuat situs SharePoint</span><span class="sxs-lookup"><span data-stu-id="a73aa-102">Create a SharePoint site</span></span>

<span data-ttu-id="a73aa-103">Membuat atau mengelola situs dari [situs aktif](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) di pusat admin SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a73aa-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="a73aa-104">Untuk informasi selengkapnya, lihat [mengelola situs di pusat admin SharePoint yang baru](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="a73aa-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="a73aa-105">Pipet</span><span class="sxs-lookup"><span data-stu-id="a73aa-105">Tips:</span></span>

- <span data-ttu-id="a73aa-106">Anda **tidak bisa** membuat situs dengan URL yang sama dari situs yang sudah ada.</span><span class="sxs-lookup"><span data-stu-id="a73aa-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="a73aa-107">Jika Anda menghapus situs dan ingin menggunakan kembali URL, mungkin situs yang dihapus masih ada di bawah [situs yang dihapus](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span><span class="sxs-lookup"><span data-stu-id="a73aa-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="a73aa-108">Situs harus dihapus secara permanen untuk menggunakan kembali URL.</span><span class="sxs-lookup"><span data-stu-id="a73aa-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="a73aa-109">Untuk menghapus situs dengan PowerShell, lihat contoh cmdlet [Remove-spsitus](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="a73aa-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="a73aa-110">Beberapa pengguna mungkin tidak bisa membuat situs.</span><span class="sxs-lookup"><span data-stu-id="a73aa-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="a73aa-111">[Lihat mengelola pembuatan situs di SharePoint online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="a73aa-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="a73aa-112">Kemungkinan situs tersebut tampak macet saat **membuat** yang lebih lama dari yang diharapkan.</span><span class="sxs-lookup"><span data-stu-id="a73aa-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="a73aa-113">Jika lebih dari 24 jam telah berlalu sejak pertama kali melihat masalah ini, silakan masuk ke tiket dukungan.</span><span class="sxs-lookup"><span data-stu-id="a73aa-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="a73aa-114">Dalam banyak kasus, kami sedang mengupayakan solusi.</span><span class="sxs-lookup"><span data-stu-id="a73aa-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="a73aa-115">Harap Beri kami setidaknya 24 jam untuk menyelesaikan solusi.</span><span class="sxs-lookup"><span data-stu-id="a73aa-115">Please give us at least 24 hours to complete a solution.</span></span>
