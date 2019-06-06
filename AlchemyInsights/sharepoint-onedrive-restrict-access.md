---
title: Membatasi akses dalam SharePoint atau OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 5101366ff65f477c19b9c7f2c0d7065cf88501b0
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/05/2019
ms.locfileid: "34735146"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="0cd17-102">Membatasi akses dalam SharePoint atau OneDrive</span><span class="sxs-lookup"><span data-stu-id="0cd17-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="0cd17-103">Ada banyak cara untuk membatasi akses ke Layanan SharePoint Online/OneDrive.</span><span class="sxs-lookup"><span data-stu-id="0cd17-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="0cd17-104">Pembatasan akses ini berbagai metode adalah sebagai berikut.</span><span class="sxs-lookup"><span data-stu-id="0cd17-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="0cd17-105">Izin pembatasan</span><span class="sxs-lookup"><span data-stu-id="0cd17-105">Permission Restriction</span></span>

<span data-ttu-id="0cd17-106">SharePoint Online dan OneDrive untuk bisnis, kami membatasi akses ke barang-barang seperti situs, file dan folder dengan hanya memberikan akses ke kelompok/individu yang harus memiliki akses.</span><span class="sxs-lookup"><span data-stu-id="0cd17-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

[<span data-ttu-id="0cd17-107">Mengubahsuaikan izin untuk daftar SharePoint atau Perpustakaan</span><span class="sxs-lookup"><span data-stu-id="0cd17-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/en-us/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

[<span data-ttu-id="0cd17-108">Mengubahsuaikan izin situs SharePoint</span><span class="sxs-lookup"><span data-stu-id="0cd17-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions)

[<span data-ttu-id="0cd17-109">Mengubah hak akses subfolder</span><span class="sxs-lookup"><span data-stu-id="0cd17-109">Change the permissions on a subfolder</span></span>](https://support.office.com/en-us/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

[<span data-ttu-id="0cd17-110">Kontrol akses dari unmanaged perangkat</span><span class="sxs-lookup"><span data-stu-id="0cd17-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/en-us/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="0cd17-111">Sebagai SharePoint atau admin global di Office 365, Anda dapat memblokir atau membatasi akses ke konten SharePoint dan OneDrive dari unmanaged perangkat (mereka tidak hibrida iklan bergabung atau compliant di Intune).</span><span class="sxs-lookup"><span data-stu-id="0cd17-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="0cd17-112">Pembatasan lokasi jaringan</span><span class="sxs-lookup"><span data-stu-id="0cd17-112">Network Location Restriction</span></span>

<span data-ttu-id="0cd17-113">Sebagai seorang IT admin, Anda dapat mengontrol akses ke sumber daya SharePoint dan OneDrive, berdasarkan jaringan didefinisikan lokasi yang Anda percaya.</span><span class="sxs-lookup"><span data-stu-id="0cd17-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="0cd17-114">Hal ini juga dikenal sebagai kebijakan berbasis lokasi.</span><span class="sxs-lookup"><span data-stu-id="0cd17-114">This is also known as location-based policy.</span></span> <span data-ttu-id="0cd17-115">Untuk informasi lebih lanjut, silakan lihat [kontrol akses ke SharePoint Online dan data OneDrive berdasarkan lokasi jaringan](https://docs.microsoft.com/en-us/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="0cd17-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/en-us/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="0cd17-116">Situs kunci pembatasan</span><span class="sxs-lookup"><span data-stu-id="0cd17-116">Site Lock Restriction</span></span> 

<span data-ttu-id="0cd17-117">Dalam SharePoint Online Anda memiliki kemampuan untuk mengunci situs koleksi, jadi tidak ada yang memiliki akses.</span><span class="sxs-lookup"><span data-stu-id="0cd17-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="0cd17-118">Ini ditetapkan melalui PowerShell dan [SharePoint Online Management Shell](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) menggunakan [Set-SPOSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) - LockState properti.</span><span class="sxs-lookup"><span data-stu-id="0cd17-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="0cd17-119">Membatasi user dari menciptakan situs atau subsites</span><span class="sxs-lookup"><span data-stu-id="0cd17-119">Restrict users from creating sites or subsites</span></span>

<span data-ttu-id="0cd17-120">Sebagai SharePoint admin atau admin global Office 365, Anda dapat membiarkan pengguna membuat dan mengelola sendiri situs SharePoint, menentukan apa jenis situs mereka dapat membuat, dan menentukan lokasi situs.</span><span class="sxs-lookup"><span data-stu-id="0cd17-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="0cd17-121">Untuk selengkapnya, lihat [mengelola situs penciptaan dalam SharePoint Online](https://docs.microsoft.com/en-us/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="0cd17-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/en-us/sharepoint/manage-site-creation)</span></span>

