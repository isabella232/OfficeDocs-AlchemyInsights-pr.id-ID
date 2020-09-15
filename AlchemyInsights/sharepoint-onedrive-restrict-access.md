---
title: Membatasi akses di SharePoint atau OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700458"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="b2ea7-102">Membatasi akses di SharePoint atau OneDrive</span><span class="sxs-lookup"><span data-stu-id="b2ea7-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="b2ea7-103">Ada banyak cara untuk membatasi akses ke Layanan SharePoint online/OneDrive.</span><span class="sxs-lookup"><span data-stu-id="b2ea7-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="b2ea7-104">Metode pembatasan akses ini diuraikan di bawah ini.</span><span class="sxs-lookup"><span data-stu-id="b2ea7-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="b2ea7-105">**Pembatasan izin**</span><span class="sxs-lookup"><span data-stu-id="b2ea7-105">**Permission Restriction**</span></span>

<span data-ttu-id="b2ea7-106">Di SharePoint online dan OneDrive for Business, kami membatasi akses ke item seperti situs, file, dan folder dengan hanya memberikan akses ke grup/individu yang seharusnya memiliki akses.</span><span class="sxs-lookup"><span data-stu-id="b2ea7-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="b2ea7-107">Mengkustomisasi izin untuk daftar atau pustaka SharePoint</span><span class="sxs-lookup"><span data-stu-id="b2ea7-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="b2ea7-108">Mengkustomisasi izin situs SharePoint</span><span class="sxs-lookup"><span data-stu-id="b2ea7-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="b2ea7-109">Mengubah izin pada subfolder</span><span class="sxs-lookup"><span data-stu-id="b2ea7-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="b2ea7-110">Mengontrol akses dari perangkat yang tidak dikelola</span><span class="sxs-lookup"><span data-stu-id="b2ea7-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="b2ea7-111">Sebagai admin SharePoint atau global, Anda dapat memblokir atau membatasi akses ke SharePoint dan konten OneDrive dari perangkat yang tidak dikelola (yang bukan iklan hibrid yang digabungkan atau patuh di Intune).</span><span class="sxs-lookup"><span data-stu-id="b2ea7-111">As a SharePoint or global admin, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="b2ea7-112">**Pembatasan lokasi jaringan**</span><span class="sxs-lookup"><span data-stu-id="b2ea7-112">**Network Location Restriction**</span></span>

<span data-ttu-id="b2ea7-113">Sebagai admin TI, Anda dapat mengontrol akses ke SharePoint dan sumber daya OneDrive berdasarkan lokasi jaringan yang Anda percayai.</span><span class="sxs-lookup"><span data-stu-id="b2ea7-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="b2ea7-114">Ini juga dikenal sebagai kebijakan berbasis lokasi.</span><span class="sxs-lookup"><span data-stu-id="b2ea7-114">This is also known as location-based policy.</span></span> <span data-ttu-id="b2ea7-115">Untuk informasi selengkapnya, lihat [mengontrol akses ke data SharePoint online dan OneDrive berdasarkan lokasi jaringan](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="b2ea7-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="b2ea7-116">**Pembatasan kunci situs**</span><span class="sxs-lookup"><span data-stu-id="b2ea7-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="b2ea7-117">Dalam SharePoint online, Anda memiliki kemampuan untuk mengunci kumpulan situs, sehingga tidak ada orang yang memiliki akses.</span><span class="sxs-lookup"><span data-stu-id="b2ea7-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="b2ea7-118">Ini diatur melalui PowerShell dan [SharePoint online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) menggunakan properti [set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate.</span><span class="sxs-lookup"><span data-stu-id="b2ea7-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="b2ea7-119">**Membatasi pengguna membuat situs atau subsitus**</span><span class="sxs-lookup"><span data-stu-id="b2ea7-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="b2ea7-120">Sebagai admin SharePoint atau admin global, Anda bisa memungkinkan pengguna Anda membuat dan mengelola situs SharePoint mereka sendiri, menentukan jenis situs yang dapat mereka buat, dan menentukan lokasi situs.</span><span class="sxs-lookup"><span data-stu-id="b2ea7-120">As a SharePoint admin or Global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="b2ea7-121">Untuk informasi selengkapnya, lihat [mengelola pembuatan situs di SharePoint online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="b2ea7-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

