---
title: Membuat situs SharePoint
ms.author: efrene
author: efrene
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 30c51d84005534cc1de9e8b8136da1a07be57b73
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/18/2019
ms.locfileid: "36738200"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="be12b-102">Membuat situs SharePoint</span><span class="sxs-lookup"><span data-stu-id="be12b-102">Create a SharePoint site</span></span>

<span data-ttu-id="be12b-103">Anda dapat melihat berikut ini untuk informasi tentang pembuatan situs SharePoint:</span><span class="sxs-lookup"><span data-stu-id="be12b-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="be12b-104">[Mengelola situs di pusat admin SharePoint baru](https://docs.microsoft.com/sharepoint/manage-site-creation): Pelajari tentang opsi pembuatan situs, termasuk cara membuat situs klasik atau situs tim yang tidak menyertakan grup Office 365.</span><span class="sxs-lookup"><span data-stu-id="be12b-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="be12b-105">[Membuat situs tim di SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Pelajari cara membuat situs tim.</span><span class="sxs-lookup"><span data-stu-id="be12b-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Learn how to create a team site.</span></span>
- <span data-ttu-id="be12b-106">[Membuat situs komunikasi di SharePoint online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Pelajari cara membuat situs komunikasi.</span><span class="sxs-lookup"><span data-stu-id="be12b-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="be12b-107">[Mengelola situs di pusat admin SharePoint baru](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): Pelajari cara membuat situs klasik atau situs tim yang tidak termasuk grup Office 365.</span><span class="sxs-lookup"><span data-stu-id="be12b-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
> <span data-ttu-id="be12b-108">[! Tips</span><span class="sxs-lookup"><span data-stu-id="be12b-108">[!Tips]</span></span>
> - <span data-ttu-id="be12b-109">Anda tidak dapat membuat situs dengan URL yang sama dari situs yang ada.</span><span class="sxs-lookup"><span data-stu-id="be12b-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="be12b-110">Jika Anda menghapus situs dan ingin menggunakan kembali URL, kemungkinan situs yang dihapus masih ada di **situs yang dihapus**.</span><span class="sxs-lookup"><span data-stu-id="be12b-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="be12b-111">Untuk mengelola situs yang dihapus, [Hapus situs](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="be12b-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="be12b-112">Untuk menghapus situs dengan PowerShell, lihat contoh [Hapus-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet.</span><span class="sxs-lookup"><span data-stu-id="be12b-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="be12b-113">Beberapa pengguna mungkin tidak dapat membuat situs.</span><span class="sxs-lookup"><span data-stu-id="be12b-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="be12b-114">Lihat [Kelola pembuatan situs di SharePoint online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="be12b-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
> - <span data-ttu-id="be12b-115">Ada kemungkinan situs muncul terjebak di **membuat** lebih lama dari yang diharapkan.</span><span class="sxs-lookup"><span data-stu-id="be12b-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="be12b-116">Jika lebih dari 24 jam telah berlalu sejak Anda pertama kali melihat masalah ini, silakan log tiket dukungan.</span><span class="sxs-lookup"><span data-stu-id="be12b-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="be12b-117">Dalam banyak kasus, kami telah bekerja pada solusi.</span><span class="sxs-lookup"><span data-stu-id="be12b-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="be12b-118">Tolong beri kami setidaknya 24 jam untuk menyelesaikan solusi.</span><span class="sxs-lookup"><span data-stu-id="be12b-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="be12b-119">Jika Anda perlu membuat situs tim baru yang tidak menyertakan grup Office 365,</span><span class="sxs-lookup"><span data-stu-id="be12b-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


