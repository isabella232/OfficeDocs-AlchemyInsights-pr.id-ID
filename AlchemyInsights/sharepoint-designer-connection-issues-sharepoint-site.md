---
title: Tingkat izin SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760696"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="57aec-102">Masalah sambungan SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="57aec-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="57aec-103">Jika SharePoint Designer mengalami masalah sambungan ke situs SharePoint, silahkan mencoba solusi umum berikut.</span><span class="sxs-lookup"><span data-stu-id="57aec-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please attempt the following common solutions.</span></span>

<span data-ttu-id="57aec-104">Langkah 1: Verifikasikan SharePoint Designer diperbarui.</span><span class="sxs-lookup"><span data-stu-id="57aec-104">Step 1: Verify SharePoint Designer is updated.</span></span>

- [<span data-ttu-id="57aec-105">SharePoint Designer 2013</span><span class="sxs-lookup"><span data-stu-id="57aec-105">SharePoint Designer 2013</span></span>](https://www.microsoft.com/download/details.aspx?id=35491)

- [<span data-ttu-id="57aec-106">SharePoint Designer Paket Layanan 1 (SP1)</span><span class="sxs-lookup"><span data-stu-id="57aec-106">SharePoint Designer Service Pack 1 (SP1)</span></span>](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [<span data-ttu-id="57aec-107">Pembaruan untuk SharePoint Designer 2013 (KB3114721)</span><span class="sxs-lookup"><span data-stu-id="57aec-107">Update for SharePoint Designer 2013 (KB3114721)</span></span>](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

<span data-ttu-id="57aec-108">Langkah 2: Kosongkan cache lokal file</span><span class="sxs-lookup"><span data-stu-id="57aec-108">Step 2: Clear the local cache files</span></span>

- <span data-ttu-id="57aec-109">Dekat SharePoint desainer 2013.</span><span class="sxs-lookup"><span data-stu-id="57aec-109">Close SharePoint Designer 2013.</span></span>

- <span data-ttu-id="57aec-110">Pada komputer lokal, browse ke folder berikut untuk menghapus cache file.</span><span class="sxs-lookup"><span data-stu-id="57aec-110">On the local computer, browse to the following folders to remove cached files.</span></span>

- <span data-ttu-id="57aec-111">Klik mulai, jalankan dan menghapus semua file yang ditemukan di bawah masing-masing di bawah lokasi.</span><span class="sxs-lookup"><span data-stu-id="57aec-111">Click Start, Run and delete all files found under each of the below locations.</span></span>

<span data-ttu-id="57aec-112">%APPDATA%\Microsoft\Web server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="57aec-112">%APPDATA%\Microsoft\Web Server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

<span data-ttu-id="57aec-113">Buka SharePoint desainer 2013 dan masukkan account lagi untuk melihat apakah ia bekerja.</span><span class="sxs-lookup"><span data-stu-id="57aec-113">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="57aec-114">Langkah 3: [mengaktifkan otentikasi Modern untuk kantor 2013 pada perangkat Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="57aec-114">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span></span>

<span data-ttu-id="57aec-115">Langkah 4: Administrator akan perlu untuk membolehkan Custom Script untuk memungkinkan koneksi SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="57aec-115">Step 4: Administrators will need to Allow Custom Script to allow the SharePoint Designer connection.</span></span>

<span data-ttu-id="57aec-116">Untuk langkah-langkah rinci, contoh dan pertimbangan Lihat [Bolehkan atau mencegah script kustom](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="57aec-116">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


