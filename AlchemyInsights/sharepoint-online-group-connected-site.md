---
title: Menambahkan grup ke situs SharePoint
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 423db4e5bbb85e75aee3548d5b6b46a64ebc6fa0
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/18/2019
ms.locfileid: "36750523"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="86f56-102">Masalah saat membuat atau grup terhubung situs di SharePoint online</span><span class="sxs-lookup"><span data-stu-id="86f56-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="86f56-103">Ada beberapa masalah umum yang dihadapi saat membuat atau membuat ulang grup situs yang terhubung.</span><span class="sxs-lookup"><span data-stu-id="86f56-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="86f56-104">Jika Anda telah menghapus grup dan situs yang terhubung dan ingin membuat situs lain dengan URL yang sama, Anda harus menghapus situs sebelumnya secara permanen.</span><span class="sxs-lookup"><span data-stu-id="86f56-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="86f56-105">Unduh [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="86f56-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="86f56-106">Untuk informasi lebih lanjut tentang memulai dengan PowerShell, lihat memulai [SharePoint online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="86f56-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="86f56-107">Menghapus situs dari situs dihapus menggunakan cmdlet PowerShell [Hapus-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="86f56-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="86f56-108">Jika Anda membuat grup situs yang terhubung dan menerima peringatan grup lain dengan alias yang sama sudah ada, periksa grup yang ada dari [Office 365 dari Pusat admin](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="86f56-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="86f56-109">Untuk mengatasi masalah ini, Hapus grup yang ada jika tidak lagi diperlukan atau membuat situs dengan alias lain yang ditetapkan.</span><span class="sxs-lookup"><span data-stu-id="86f56-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="86f56-110">Ada berbagai cara untuk membuat dan menggunakan grup modern dengan SharePoint.</span><span class="sxs-lookup"><span data-stu-id="86f56-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="86f56-111">Anda dapat menghubungkan situs yang ada ke grup 365 Office.</span><span class="sxs-lookup"><span data-stu-id="86f56-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="86f56-112">Untuk informasi lebih lanjut, lihat [menyambungkan grup 365 Office menggunakan pengguna SharePoint ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="86f56-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="86f56-113">Untuk membuat situs Office 365 grup yang terhubung, Anda harus membuat situs tim.</span><span class="sxs-lookup"><span data-stu-id="86f56-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="86f56-114">Untuk informasi lebih lanjut, lihat [membuat tim situs di SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="86f56-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

