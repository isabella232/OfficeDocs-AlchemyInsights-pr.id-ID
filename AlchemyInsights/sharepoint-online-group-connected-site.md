---
title: Menambahkan grup ke situs SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 049ef5acd80d64e00315ba07f274567e6a251904
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/21/2020
ms.locfileid: "43642147"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="b6a89-102">Masalah saat membuat grup terhubung situs di SharePoint</span><span class="sxs-lookup"><span data-stu-id="b6a89-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="b6a89-103">Beberapa masalah umum yang dihadapi saat membuat atau membuat ulang grup situs yang terhubung.</span><span class="sxs-lookup"><span data-stu-id="b6a89-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="b6a89-104">Jika Anda telah menghapus grup dan situs yang terhubung dan ingin membuat situs lain dengan URL yang sama, Anda harus menghapus situs sebelumnya secara permanen.</span><span class="sxs-lookup"><span data-stu-id="b6a89-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="b6a89-105">Unduh [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="b6a89-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="b6a89-106">Untuk informasi lebih lanjut tentang cara memulai dengan PowerShell, lihat memulai [SharePoint online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="b6a89-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="b6a89-107">Menghapus situs dari situs dihapus menggunakan cmdlet PowerShell [Hapus-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="b6a89-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="b6a89-108">PowerShell diperlukan untuk menghapus secara permanen situs grup.</span><span class="sxs-lookup"><span data-stu-id="b6a89-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="b6a89-109">Jika Anda membuat grup situs yang terhubung dan menerima peringatan: **grup lain dengan alias yang sama sudah ada**, periksa grup yang ada dari [pusat admin Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="b6a89-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="b6a89-110">Untuk mengatasi masalah ini, Hapus grup yang ada jika tidak lagi diperlukan atau membuat situs dengan alias lain yang ditetapkan.</span><span class="sxs-lookup"><span data-stu-id="b6a89-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="b6a89-111">Ada berbagai cara untuk membuat dan menggunakan grup modern dengan SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b6a89-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="b6a89-112">Anda dapat menghubungkan situs yang ada ke grup 365 Office.</span><span class="sxs-lookup"><span data-stu-id="b6a89-112">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="b6a89-113">Untuk informasi lebih lanjut, lihat [menyambungkan grup 365 Office menggunakan antarmuka pengguna SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="b6a89-113">For more info, see [Connect an Office 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="b6a89-114">Untuk membuat situs yang terhubung ke grup Office 365, Anda harus membuat [situs tim](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="b6a89-114">To create an Office 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
