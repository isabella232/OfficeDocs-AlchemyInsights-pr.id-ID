---
title: Membatasi akses di SharePoint atau OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: bef0612903b9bb455aa34e90d35d6b7b9093b4e0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750667"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="f04b6-102">Membatasi akses di SharePoint atau OneDrive</span><span class="sxs-lookup"><span data-stu-id="f04b6-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="f04b6-103">Ada banyak cara untuk membatasi akses ke SharePoint online/Layanan OneDrive.</span><span class="sxs-lookup"><span data-stu-id="f04b6-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="f04b6-104">Ini berbagai metode pembatasan akses diuraikan di bawah ini.</span><span class="sxs-lookup"><span data-stu-id="f04b6-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="f04b6-105">**Pembatasan izin**</span><span class="sxs-lookup"><span data-stu-id="f04b6-105">**Permission Restriction**</span></span>

<span data-ttu-id="f04b6-106">Di SharePoint online dan OneDrive for Business, kami membatasi akses ke item seperti situs, file, dan folder hanya dengan memberikan akses ke grup/individu yang seharusnya memiliki akses.</span><span class="sxs-lookup"><span data-stu-id="f04b6-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="f04b6-107">Menyesuaikan izin untuk SharePoint daftar atau Perpustakaan</span><span class="sxs-lookup"><span data-stu-id="f04b6-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="f04b6-108">Menyesuaikan izin situs SharePoint</span><span class="sxs-lookup"><span data-stu-id="f04b6-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="f04b6-109">Mengubah izin pada subfolder</span><span class="sxs-lookup"><span data-stu-id="f04b6-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="f04b6-110">Mengontrol akses dari perangkat yang tidak dikelola</span><span class="sxs-lookup"><span data-stu-id="f04b6-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="f04b6-111">Sebagai SharePoint atau global admin di Office 365, Anda dapat memblokir atau membatasi akses ke SharePoint dan OneDrive konten dari perangkat yang tidak dikelola (yang tidak hibrida AD bergabung atau sesuai di Intune).</span><span class="sxs-lookup"><span data-stu-id="f04b6-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="f04b6-112">**Pembatasan lokasi jaringan**</span><span class="sxs-lookup"><span data-stu-id="f04b6-112">**Network Location Restriction**</span></span>

<span data-ttu-id="f04b6-113">Sebagai admin IT, Anda dapat mengontrol akses ke sumber daya SharePoint dan OneDrive berdasarkan lokasi jaringan yang ditentukan yang Anda percayai.</span><span class="sxs-lookup"><span data-stu-id="f04b6-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="f04b6-114">Ini juga dikenal sebagai kebijakan berbasis lokasi.</span><span class="sxs-lookup"><span data-stu-id="f04b6-114">This is also known as location-based policy.</span></span> <span data-ttu-id="f04b6-115">Untuk informasi selengkapnya, silakan lihat [kontrol akses ke SharePoint online dan data OneDrive berdasarkan lokasi jaringan](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="f04b6-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="f04b6-116">**Pembatasan kunci situs**</span><span class="sxs-lookup"><span data-stu-id="f04b6-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="f04b6-117">Dalam SharePoint online Anda memiliki kemampuan untuk mengunci koleksi situs, sehingga tidak ada yang memiliki akses.</span><span class="sxs-lookup"><span data-stu-id="f04b6-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="f04b6-118">Ini diatur melalui PowerShell dan [SharePoint online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) menggunakan properti [set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate.</span><span class="sxs-lookup"><span data-stu-id="f04b6-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="f04b6-119">**Membatasi pengguna membuat situs atau subsitus**</span><span class="sxs-lookup"><span data-stu-id="f04b6-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="f04b6-120">Sebagai admin SharePoint atau admin global 365 Office, Anda dapat membiarkan pengguna membuat dan mengelola situs SharePoint mereka sendiri, menentukan jenis situs yang dapat mereka buat, dan menentukan lokasi situs.</span><span class="sxs-lookup"><span data-stu-id="f04b6-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="f04b6-121">Untuk informasi lebih lanjut, silakan lihat [Kelola pembuatan situs di SharePoint online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="f04b6-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

