---
title: Buka dengan Explorer tidak bekerja
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: b55fc7bd5670e655334ef7be368b245c8899633a
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/15/2019
ms.locfileid: "28294414"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="c36c5-102">Buka dengan Explorer tidak bekerja</span><span class="sxs-lookup"><span data-stu-id="c36c5-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="c36c5-p101">Jika **terbuka dengan Explorer** atau **lihat di File Explorer** tidak berfungsi pastikan layanan WebClient diatur untuk **menjalankan** dengan mengikuti langkah-langkah berikut. Sebagai contoh, itu mungkin memakan waktu lama untuk membuka perpustakaan SharePoint atau OneDrive ketika Layanan tidak berjalan.</span><span class="sxs-lookup"><span data-stu-id="c36c5-p101">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below. For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="c36c5-105">Di kotak pencarian Windows, menjalankan, jenis pilih aplikasi desktop jalankan, ketik services.msc, dan kemudian pilih **Enter**.</span><span class="sxs-lookup"><span data-stu-id="c36c5-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="c36c5-p102">Gulir ke bawah ke layanan WebClient dan memeriksa kolom **Status** . Jika status layanan WebClient tidak **menjalankan**, klik dua kali layanan, klik **mulai**, dan kemudian klik **OK**. Mengaktifkan layanan, jika diperlukan, dengan memilih baik **Manual** atau **otomatis** di kotak **Startup type** .</span><span class="sxs-lookup"><span data-stu-id="c36c5-p102">Scroll down to the WebClient service and check the **Status** column. If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**. Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="c36c5-p103">Untuk memecahkan masalah membuka File Explorer, lihat [terbuka di Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Jelajahi sync sebagai alternatif yang lebih baik: [Sync SharePoint file dengan OneDrive sync klien baru](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="c36c5-p103">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

