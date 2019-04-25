---
title: Buka dengan Explorer tidak bekerja
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 73d33e50449345c312abdd39afcc36e0c95fd1c4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/23/2019
ms.locfileid: "32419875"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="84faa-102">Buka dengan Explorer tidak bekerja</span><span class="sxs-lookup"><span data-stu-id="84faa-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="84faa-103">Jika **terbuka dengan Explorer** atau **lihat di File Explorer** tidak berfungsi pastikan layanan WebClient diatur untuk **menjalankan** dengan mengikuti langkah-langkah berikut.</span><span class="sxs-lookup"><span data-stu-id="84faa-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="84faa-104">Sebagai contoh, itu mungkin memakan waktu lama untuk membuka perpustakaan SharePoint atau OneDrive ketika Layanan tidak berjalan.</span><span class="sxs-lookup"><span data-stu-id="84faa-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="84faa-105">Di kotak pencarian Windows, menjalankan, jenis pilih aplikasi desktop jalankan, ketik services.msc, dan kemudian pilih **Enter**.</span><span class="sxs-lookup"><span data-stu-id="84faa-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="84faa-106">Gulir ke bawah ke layanan WebClient dan memeriksa kolom **Status** .</span><span class="sxs-lookup"><span data-stu-id="84faa-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="84faa-107">Jika status layanan WebClient tidak **menjalankan**, klik dua kali layanan, klik **mulai**, dan kemudian klik **OK**.</span><span class="sxs-lookup"><span data-stu-id="84faa-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="84faa-108">Mengaktifkan layanan, jika diperlukan, dengan memilih baik **Manual** atau **otomatis** di kotak **Startup type** .</span><span class="sxs-lookup"><span data-stu-id="84faa-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="84faa-109">Untuk memecahkan masalah membuka File Explorer, lihat [terbuka di Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="84faa-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="84faa-110">Jelajahi sync sebagai alternatif yang lebih baik: [Sync SharePoint file dengan OneDrive sync klien baru](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="84faa-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

