---
title: Membuat situs SharePoint
ms.author: pebaum
author: todmccoy
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
ms.openlocfilehash: e1e71ae9401448ed18058f6307302dcbaf773649
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770858"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="45e82-102">Membuat situs SharePoint</span><span class="sxs-lookup"><span data-stu-id="45e82-102">Create a SharePoint site</span></span>

<span data-ttu-id="45e82-103">Membuat atau mengelola situs dari [situs aktif](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) di pusat admin SharePoint.</span><span class="sxs-lookup"><span data-stu-id="45e82-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="45e82-104">Untuk informasi lebih lanjut, lihat [mengelola situs di pusat admin SharePoint baru](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="45e82-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="45e82-105">Tips:</span><span class="sxs-lookup"><span data-stu-id="45e82-105">Tips:</span></span>

- <span data-ttu-id="45e82-106">Anda **tidak dapat** membuat situs dengan URL yang sama dari situs yang ada.</span><span class="sxs-lookup"><span data-stu-id="45e82-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="45e82-107">Jika Anda menghapus situs dan ingin menggunakan kembali URL, kemungkinan situs yang dihapus masih ada di [situs yang dihapus](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span><span class="sxs-lookup"><span data-stu-id="45e82-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="45e82-108">Situs harus dihapus secara permanen untuk menggunakan kembali URL.</span><span class="sxs-lookup"><span data-stu-id="45e82-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="45e82-109">Untuk menghapus situs dengan PowerShell, lihat contoh [Hapus-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet.</span><span class="sxs-lookup"><span data-stu-id="45e82-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="45e82-110">Beberapa pengguna mungkin tidak dapat membuat situs.</span><span class="sxs-lookup"><span data-stu-id="45e82-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="45e82-111">[Lihat Kelola pembuatan situs di SharePoint online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="45e82-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="45e82-112">Ada kemungkinan situs muncul terjebak di **membuat** lebih lama dari yang diharapkan.</span><span class="sxs-lookup"><span data-stu-id="45e82-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="45e82-113">Jika lebih dari 24 jam telah berlalu sejak Anda pertama kali melihat masalah ini, silakan log tiket dukungan.</span><span class="sxs-lookup"><span data-stu-id="45e82-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="45e82-114">Dalam banyak kasus, kami telah bekerja pada solusi.</span><span class="sxs-lookup"><span data-stu-id="45e82-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="45e82-115">Tolong beri kami setidaknya 24 jam untuk menyelesaikan solusi.</span><span class="sxs-lookup"><span data-stu-id="45e82-115">Please give us at least 24 hours to complete a solution.</span></span>
