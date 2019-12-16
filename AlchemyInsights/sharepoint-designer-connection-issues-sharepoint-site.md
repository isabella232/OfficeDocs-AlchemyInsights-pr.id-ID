---
title: Masalah sambungan SharePoint Designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 9730bd66afd494385db3de605f5fe68d0f274ed3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051716"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="69c2f-102">Masalah sambungan SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="69c2f-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="69c2f-103">Jika SharePoint Designer mengalami masalah sambungan ke situs SharePoint, silakan coba solusi umum berikut ini.</span><span class="sxs-lookup"><span data-stu-id="69c2f-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="69c2f-104">Langkah 1: verifikasi bahwa 2013 SharePoint Designer diperbarui dengan [SharePoint Designer Paket Layanan 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) dan [2 Agustus 2016 pemutakhiran untuk 2013 Designer SharePoint](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="69c2f-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="69c2f-105">Langkah 2: Kosongkan file cache lokal:</span><span class="sxs-lookup"><span data-stu-id="69c2f-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="69c2f-106">Tutup SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="69c2f-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="69c2f-107">Pada komputer lokal, Hapus semua berkas yang ditemukan di setiap folder berikut ini.</span><span class="sxs-lookup"><span data-stu-id="69c2f-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="69c2f-108">%APPDATA%\Microsoft\Web server Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="69c2f-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="69c2f-109">% AppData%\microsoft\sharepoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="69c2f-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="69c2f-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="69c2f-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="69c2f-111">Buka SharePoint Designer 2013 dan masukkan akun lagi untuk melihat apakah ia bekerja.</span><span class="sxs-lookup"><span data-stu-id="69c2f-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="69c2f-112">Langkah 3: [aktifkan otentikasi modern untuk Office 2013 pada perangkat Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="69c2f-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span></span>

<span data-ttu-id="69c2f-113">Langkah 4: Administrator akan perlu untuk **mengizinkan skrip kustom** di Tataan Pusat admin SharePoint untuk mengizinkan sambungan SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="69c2f-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="69c2f-114">Lihat [membolehkan atau mencegah skrip kustom](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) untuk informasi lebih lanjut.</span><span class="sxs-lookup"><span data-stu-id="69c2f-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


