---
title: Memecahkan masalah menggunakan terbuka dengan Explorer
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 03bb3ad01a716390ec50845b29ddf6cc81a83116
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/22/2019
ms.locfileid: "30759297"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="9b4e4-102">Memperbaiki masalah dengan terbuka dengan Explorer</span><span class="sxs-lookup"><span data-stu-id="9b4e4-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="9b4e4-103">Memperbaiki masalah umum dengan membuka pustaka dokumen di SharePoint atau OneDrive menggunakan perintah **terbuka dengan Explorer** :</span><span class="sxs-lookup"><span data-stu-id="9b4e4-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="9b4e4-104">Gunakan Internet Explorer 10 atau Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="9b4e4-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="9b4e4-105">**Terbuka dengan Explorer** tidak kompatibel dengan Microsoft Edge, Google Chrome, Firefox, dan lain-lain.</span><span class="sxs-lookup"><span data-stu-id="9b4e4-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="9b4e4-106">**Terbuka dengan Explorer** dinonaktifkan di semua browser kecuali Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="9b4e4-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="9b4e4-107">**Terbuka dengan Explorer** ini tidak tersedia dalam pengalaman modern untuk SharePoint Perpustakaan.</span><span class="sxs-lookup"><span data-stu-id="9b4e4-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="9b4e4-108">Menggunakan **tampilan di File Explorer** sebagai gantinya.</span><span class="sxs-lookup"><span data-stu-id="9b4e4-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="9b4e4-109">Pilih **opsi tampilan** \> **pandangan dalam File Explorer**.</span><span class="sxs-lookup"><span data-stu-id="9b4e4-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="9b4e4-110">Lihat di File Explorer tidak kompatibel dengan Microsoft Edge, Google Chrome, Firefox, dan lain-lain.</span><span class="sxs-lookup"><span data-stu-id="9b4e4-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="9b4e4-111">**Tampilan di File Explorer** di tersedia hanya di Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="9b4e4-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="9b4e4-112">Pastikan Layanan WebClient berjalan.</span><span class="sxs-lookup"><span data-stu-id="9b4e4-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="9b4e4-113">Di kotak pencarian Windows, ketik dijalankan, pilih aplikasi desktop jalankan, ketik services.msc, dan kemudian tekan Enter.</span><span class="sxs-lookup"><span data-stu-id="9b4e4-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="9b4e4-114">Gulir ke bawah untuk WebClient layanan dan pastikan kolom **Status** menampilkan "Berjalan."</span><span class="sxs-lookup"><span data-stu-id="9b4e4-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="9b4e4-115">Jika tidak, klik dua kali layanan, klik **mulai**, dan kemudian klik **OK**.</span><span class="sxs-lookup"><span data-stu-id="9b4e4-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="9b4e4-116">(Anda mungkin perlu terlebih dahulu mengaktifkan layanan dengan memilih baik **Manual** atau **otomatis** di kotak **Startup type** .)</span><span class="sxs-lookup"><span data-stu-id="9b4e4-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="9b4e4-117">Membuka sebuah perpustakaan di File Explorer berguna jika Anda perlu untuk menyalin atau memindahkan beberapa file dan folder sekali, tetapi jika Anda ingin secara teratur bekerja di Perpustakaan, sebaiknya sinkronisasi.</span><span class="sxs-lookup"><span data-stu-id="9b4e4-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="9b4e4-118">Untuk memecahkan masalah membuka File Explorer, lihat [terbuka di Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="9b4e4-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="9b4e4-119">Untuk info tentang cara mengatur sinkronisasi, lihat [Sync SharePoint file dengan OneDrive sync klien baru](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="9b4e4-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="9b4e4-120">Silakan lihat artikel [bagaimana menggunakan perintah "terbuka dengan Explorer" untuk memecahkan masalah di SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) untuk informasi lebih lanjut.</span><span class="sxs-lookup"><span data-stu-id="9b4e4-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) for more information.</span></span> 
  

