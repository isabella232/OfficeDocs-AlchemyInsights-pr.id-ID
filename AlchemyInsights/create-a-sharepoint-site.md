---
title: Buat situs SharePoint
ms.author: kirks
author: Techwriter40
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1386"
- "2303"
- "5200004"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 022f572aadae3b4d9f6665f9f8be871d79b51817
ms.sourcegitcommit: f81c56dd4ae7cb2eedc383dd671b9012f3089286
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/19/2019
ms.locfileid: "35802969"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="71d72-102">Buat situs SharePoint</span><span class="sxs-lookup"><span data-stu-id="71d72-102">Create a SharePoint site</span></span>

<span data-ttu-id="71d72-103">Anda dapat melihat berikut untuk informasi tentang pembuatan situs SharePoint:</span><span class="sxs-lookup"><span data-stu-id="71d72-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="71d72-104">[Mengelola situs di SharePoint admin center baru](https://docs.microsoft.com/sharepoint/manage-site-creation): Pelajari tentang pilihan pembuatan situs, termasuk cara membuat situs klasik atau situs tim yang tidak mencakup grup Office 365.</span><span class="sxs-lookup"><span data-stu-id="71d72-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="71d72-105">[Buat situs tim di SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Pelajari cara membuat situs tim.</span><span class="sxs-lookup"><span data-stu-id="71d72-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Learn how to create a team site.</span></span>
- <span data-ttu-id="71d72-106">[Membuat sebuah situs komunikasi di SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Pelajari cara membuat sebuah situs komunikasi.</span><span class="sxs-lookup"><span data-stu-id="71d72-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="71d72-107">[Mengelola situs di SharePoint admin center baru](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): Pelajari cara membuat situs klasik atau situs tim yang tidak mencakup grup Office 365.</span><span class="sxs-lookup"><span data-stu-id="71d72-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
> [! Tips]
> - <span data-ttu-id="71d72-109">Anda tidak dapat membuat sebuah situs dengan URL yang sama dari situs yang ada.</span><span class="sxs-lookup"><span data-stu-id="71d72-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="71d72-110">Jika Anda menghapus situs dan berharap untuk kembali menggunakan URL, sangat mungkin situs dihapus masih ada di bawah **situs dihapus**.</span><span class="sxs-lookup"><span data-stu-id="71d72-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="71d72-111">Untuk mengelola dihapus lihat situs, [menghapus situs](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="71d72-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="71d72-112">Untuk menghapus sebuah situs dengan Powershell, lihat contoh cmdlet [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="71d72-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="71d72-113">Beberapa pengguna tidak dapat membuat sebuah situs.</span><span class="sxs-lookup"><span data-stu-id="71d72-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="71d72-114">Lihat [mengelola situs penciptaan dalam SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="71d72-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
> - <span data-ttu-id="71d72-115">Hal ini memungkinkan situs muncul terjebak di **membuat** lebih lama dari yang diharapkan.</span><span class="sxs-lookup"><span data-stu-id="71d72-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="71d72-116">Jika lebih dari 24 jam telah berlalu sejak Anda pertama kali melihat masalah ini, silakan log tiket support.</span><span class="sxs-lookup"><span data-stu-id="71d72-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="71d72-117">Dalam banyak kasus, kami sudah bekerja pada sebuah solusi.</span><span class="sxs-lookup"><span data-stu-id="71d72-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="71d72-118">Mohon berikan setidaknya 24 jam untuk menyelesaikan solusi.</span><span class="sxs-lookup"><span data-stu-id="71d72-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="71d72-119">Jika Anda perlu untuk membuat situs tim baru yang tidak mencakup grup Office 365</span><span class="sxs-lookup"><span data-stu-id="71d72-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


