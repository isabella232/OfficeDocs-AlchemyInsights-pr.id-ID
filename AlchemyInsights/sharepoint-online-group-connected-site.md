---
title: Menambahkan grup ke situs SharePoint
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: f0126f7f753275e9bbf8c3a09a6af5faf9a27862
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758734"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a><span data-ttu-id="a3dc6-102">Membuat situs terhubung group di SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="a3dc6-102">Create group connected site in SharePoint Online</span></span>

<span data-ttu-id="a3dc6-103">Ada beberapa masalah umum yang dihadapi ketika membuat atau menciptakan kembali kelompok yang terhubung situs.</span><span class="sxs-lookup"><span data-stu-id="a3dc6-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="a3dc6-104">Jika Anda telah menghapus grup dan situs yang terhubung dan ingin membuat situs lain dengan URL yang sama, Anda akan perlu untuk secara permanen menghapus situs sebelumnya.</span><span class="sxs-lookup"><span data-stu-id="a3dc6-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="a3dc6-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="a3dc6-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="a3dc6-106">Untuk info lebih lanjut tentang memulai dengan powershell, lihat [persiapan dengan SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="a3dc6-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="a3dc6-107">Menghapus situs dari situs dihapus menggunakan cmdlet powershell [Hapus-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="a3dc6-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="a3dc6-108">Jika Anda membuat situs terhubung group dan menerima peringatan kelompok lain dengan nama alias yang sama sudah ada, periksa grup dari [Office 365 dari Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="a3dc6-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="a3dc6-109">Untuk menyelesaikan masalah, menghapus grup yang ada jika tidak lagi diperlukan atau membuat situs dengan alias lain ditetapkan.</span><span class="sxs-lookup"><span data-stu-id="a3dc6-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="a3dc6-110">Ada berbagai cara untuk membuat dan menggunakan grup modern dengan SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a3dc6-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="a3dc6-111">Anda dapat menghubungkan situs yang ada untuk grup Office 365.</span><span class="sxs-lookup"><span data-stu-id="a3dc6-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="a3dc6-112">Untuk info lebih lanjut, lihat [Connect grup Office 365 menggunakan SharePoint pengguna ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="a3dc6-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="a3dc6-113">Untuk membuat situs terhubung group Office 365, Anda harus membuat situs tim.</span><span class="sxs-lookup"><span data-stu-id="a3dc6-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="a3dc6-114">Untuk info lebih lanjut, lihat [membuat situs tim di SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="a3dc6-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

