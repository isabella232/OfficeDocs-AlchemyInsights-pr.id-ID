---
title: Membatasi akses di SharePoint atau OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 39aa8cd6e649eca4a1e196eeb589a825364d0977
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692768"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="e45ba-102">Membatasi akses di SharePoint atau OneDrive</span><span class="sxs-lookup"><span data-stu-id="e45ba-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="e45ba-103">Ada banyak cara untuk membatasi akses ke SharePoint online/Layanan OneDrive.</span><span class="sxs-lookup"><span data-stu-id="e45ba-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="e45ba-104">Ini berbagai metode pembatasan akses diuraikan di bawah ini.</span><span class="sxs-lookup"><span data-stu-id="e45ba-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="e45ba-105">**Pembatasan izin**</span><span class="sxs-lookup"><span data-stu-id="e45ba-105">**Permission Restriction**</span></span>

<span data-ttu-id="e45ba-106">Di SharePoint online dan OneDrive for Business, kami membatasi akses ke item seperti situs, file, dan folder hanya dengan memberikan akses ke grup/individu yang seharusnya memiliki akses.</span><span class="sxs-lookup"><span data-stu-id="e45ba-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="e45ba-107">Menyesuaikan izin untuk SharePoint daftar atau Perpustakaan</span><span class="sxs-lookup"><span data-stu-id="e45ba-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="e45ba-108">Menyesuaikan izin situs SharePoint</span><span class="sxs-lookup"><span data-stu-id="e45ba-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="e45ba-109">Mengubah izin pada subfolder</span><span class="sxs-lookup"><span data-stu-id="e45ba-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="e45ba-110">Mengontrol akses dari perangkat yang tidak dikelola</span><span class="sxs-lookup"><span data-stu-id="e45ba-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="e45ba-111">Sebagai SharePoint atau global admin, Anda dapat memblokir atau membatasi akses ke SharePoint dan OneDrive konten dari perangkat yang tidak dikelola (mereka tidak hibrid AD bergabung atau sesuai di Intune).</span><span class="sxs-lookup"><span data-stu-id="e45ba-111">As a SharePoint or global admin, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="e45ba-112">**Pembatasan lokasi jaringan**</span><span class="sxs-lookup"><span data-stu-id="e45ba-112">**Network Location Restriction**</span></span>

<span data-ttu-id="e45ba-113">Sebagai admin IT, Anda dapat mengontrol akses ke sumber daya SharePoint dan OneDrive berdasarkan lokasi jaringan yang ditentukan yang Anda percayai.</span><span class="sxs-lookup"><span data-stu-id="e45ba-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="e45ba-114">Ini juga dikenal sebagai kebijakan berbasis lokasi.</span><span class="sxs-lookup"><span data-stu-id="e45ba-114">This is also known as location-based policy.</span></span> <span data-ttu-id="e45ba-115">Untuk informasi selengkapnya, silakan lihat [kontrol akses ke SharePoint online dan data OneDrive berdasarkan lokasi jaringan](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="e45ba-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="e45ba-116">**Pembatasan kunci situs**</span><span class="sxs-lookup"><span data-stu-id="e45ba-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="e45ba-117">Dalam SharePoint online Anda memiliki kemampuan untuk mengunci koleksi situs, sehingga tidak ada yang memiliki akses.</span><span class="sxs-lookup"><span data-stu-id="e45ba-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="e45ba-118">Ini diatur melalui PowerShell dan [SharePoint online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) menggunakan properti [set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate.</span><span class="sxs-lookup"><span data-stu-id="e45ba-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="e45ba-119">**Membatasi pengguna membuat situs atau subsitus**</span><span class="sxs-lookup"><span data-stu-id="e45ba-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="e45ba-120">Sebagai admin SharePoint atau global admin, Anda dapat membiarkan pengguna Anda membuat dan mengelola situs SharePoint mereka sendiri, menentukan jenis situs yang mereka dapat membuat, dan menentukan lokasi situs.</span><span class="sxs-lookup"><span data-stu-id="e45ba-120">As a SharePoint admin or Global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="e45ba-121">Untuk informasi lebih lanjut, silakan lihat [Kelola pembuatan situs di SharePoint online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="e45ba-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

