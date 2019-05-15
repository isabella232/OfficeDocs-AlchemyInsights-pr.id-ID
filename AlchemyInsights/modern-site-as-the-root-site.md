---
title: Situs modern sebagai situs akar
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057727"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="47ee1-102">Situs modern sebagai situs akar</span><span class="sxs-lookup"><span data-stu-id="47ee1-102">Modern site as root site</span></span>

<span data-ttu-id="47ee1-103">[Target Release](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) pelanggan sekarang dapat mengaktifkan pengalaman situs modern komunikasi di situs klasik akar penyewa SharePoint mereka.</span><span class="sxs-lookup"><span data-stu-id="47ee1-103">[Target Release](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) customers can now enable the modern communication site experience at the classic root site of their SharePoint tenant.</span></span>

<span data-ttu-id="47ee1-104">Fitur ini dapat diaktifkan dengan menjalankan cmdlet PowerShell sederhana.</span><span class="sxs-lookup"><span data-stu-id="47ee1-104">This feature can be activated by running a simple PowerShell cmdlet.</span></span> <span data-ttu-id="47ee1-105">Pada keberhasilan pelaksanaan PowerShell command(s), situs akar akan memiliki halaman rumah situs komunikasi baru.</span><span class="sxs-lookup"><span data-stu-id="47ee1-105">On the successful execution of the PowerShell command(s), the root site will have a new communication site home page.</span></span> <span data-ttu-id="47ee1-106">Rincian tentang persyaratan PowerShell cmdlet dan fitur tersedia dalam artikel [Aktifkan-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="47ee1-106">Details about the PowerShell cmdlet and feature requirements are available in the article [Enable-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span></span> 

<span data-ttu-id="47ee1-107">Kita akan secara bertahap rolling hal ini, off secara default, untuk pelanggan yang ditargetkan rilis di awal Mei 2019 dan gulungan keluar akan tersedia di seluruh dunia oleh akhir Juni 2019.</span><span class="sxs-lookup"><span data-stu-id="47ee1-107">We'll be gradually rolling this out, off by default, to Targeted Release customers in early May 2019, and the roll out will be available worldwide by the end of June 2019.</span></span> <span data-ttu-id="47ee1-108">Lanjutkan untuk merujuk kepada [Pusat pesan](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) fitur baru lainnya dengan Modern.</span><span class="sxs-lookup"><span data-stu-id="47ee1-108">Continue to refer to the [Message Center](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) for other new features with Modern.</span></span> 

<span data-ttu-id="47ee1-109">**Penting**: Jangan menghapus situs akar klasik untuk membuat situs komunikasi modern.</span><span class="sxs-lookup"><span data-stu-id="47ee1-109">**Important**: Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="47ee1-110">Hal ini tidak didukung oleh Microsoft.</span><span class="sxs-lookup"><span data-stu-id="47ee1-110">This is not supported by Microsoft.</span></span> <span data-ttu-id="47ee1-111">Menghapus situs akar akan membuat semua situs SharePoint dalam organisasi Anda tidak dapat diakses untuk semua pengguna, sampai Anda mengembalikan situs atau membuat situs baru di URL yang sama.</span><span class="sxs-lookup"><span data-stu-id="47ee1-111">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> 
 
 