---
title: Buka dengan Explorer tidak berfungsi
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694459"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="4bf87-102">Buka dengan Explorer tidak berfungsi</span><span class="sxs-lookup"><span data-stu-id="4bf87-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="4bf87-103">Jika **buka dengan Explorer** atau **tampilan di file Explorer** tidak berfungsi, pastikan layanan WebClient diatur agar **berjalan** dengan mengikuti langkah-langkah di bawah ini.</span><span class="sxs-lookup"><span data-stu-id="4bf87-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="4bf87-104">Misalnya, mungkin memerlukan waktu lama untuk membuka pustaka SharePoint atau OneDrive saat Layanan tidak berjalan.</span><span class="sxs-lookup"><span data-stu-id="4bf87-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="4bf87-105">Dalam kotak pencarian Windows, ketik jalankan, pilih Jalankan aplikasi desktop, ketikkan Services. MSC, lalu pilih **Enter**.</span><span class="sxs-lookup"><span data-stu-id="4bf87-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="4bf87-106">Gulir ke bawah ke layanan WebClient dan periksa kolom **status** .</span><span class="sxs-lookup"><span data-stu-id="4bf87-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="4bf87-107">Jika status layanan WebClient tidak **berjalan**, klik ganda Layanan tersebut, klik **mulai**, lalu klik **OK**.</span><span class="sxs-lookup"><span data-stu-id="4bf87-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="4bf87-108">Aktifkan layanan, jika diperlukan, dengan memilih **manual** atau **otomatis** dalam kotak **tipe startup** .</span><span class="sxs-lookup"><span data-stu-id="4bf87-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="4bf87-109">Untuk memecahkan masalah yang dibuka di file Explorer, lihat [membuka di Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="4bf87-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="4bf87-110">Jelajahi sinkronisasi sebagai alternatif yang lebih baik: [sinkronkan file SharePoint dengan klien sinkronisasi OneDrive yang baru](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="4bf87-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

