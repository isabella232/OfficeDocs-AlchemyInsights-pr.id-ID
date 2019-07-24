---
title: Masalah sambungan SharePoint Designer
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 1d3f6ad3128292a9dbcc46cc7da23af59a63fbb4
ms.sourcegitcommit: a285c609319ade038461e090e14a701830031825
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840554"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="0f7db-102">Masalah sambungan SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="0f7db-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="0f7db-103">Jika SharePoint Designer mengalami masalah sambungan ke situs SharePoint, coba solusi berikut umum.</span><span class="sxs-lookup"><span data-stu-id="0f7db-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="0f7db-104">Langkah 1: Verifikasikan bahwa SharePoint desainer 2013 diperbarui dengan [SharePoint desainer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) dan [2 Agustus 2016 pembaruan untuk SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="0f7db-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="0f7db-105">Langkah 2: Menghapus file cache lokal:</span><span class="sxs-lookup"><span data-stu-id="0f7db-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="0f7db-106">Dekat SharePoint desainer 2013.</span><span class="sxs-lookup"><span data-stu-id="0f7db-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="0f7db-107">Pada komputer lokal, menghapus semua file yang ditemukan di setiap folder berikut.</span><span class="sxs-lookup"><span data-stu-id="0f7db-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="0f7db-108">%APPDATA%\Microsoft\Web server Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="0f7db-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="0f7db-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="0f7db-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="0f7db-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="0f7db-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="0f7db-111">Buka SharePoint desainer 2013 dan masukkan account lagi untuk melihat apakah ia bekerja.</span><span class="sxs-lookup"><span data-stu-id="0f7db-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="0f7db-112">Langkah 3: [mengaktifkan otentikasi Modern untuk kantor 2013 pada perangkat Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="0f7db-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span></span>

<span data-ttu-id="0f7db-113">Langkah 4: Administrator akan perlu untuk **Membolehkan Custom Script** dalam pengaturan SharePoint Admin Center untuk memungkinkan koneksi SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="0f7db-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="0f7db-114">Lihat [Bolehkan atau mencegah script kustom](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) untuk informasi lebih lanjut.</span><span class="sxs-lookup"><span data-stu-id="0f7db-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


