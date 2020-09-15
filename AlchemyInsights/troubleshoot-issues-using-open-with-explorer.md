---
title: Memecahkan masalah menggunakan buka dengan Explorer
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659061"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="74395-102">Memperbaiki masalah saat membuka dengan Explorer</span><span class="sxs-lookup"><span data-stu-id="74395-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="74395-103">Perbaiki masalah umum dengan membuka pustaka dokumen di SharePoint atau OneDrive menggunakan perintah **buka dengan Explorer** :</span><span class="sxs-lookup"><span data-stu-id="74395-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="74395-104">Gunakan Internet Explorer 10 atau Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="74395-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="74395-105">**Buka dengan Explorer** tidak kompatibel dengan Microsoft Edge, Google Chrome, Firefox dan lainnya.</span><span class="sxs-lookup"><span data-stu-id="74395-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="74395-106">**Buka dengan Explorer** dinonaktifkan di semua browser kecuali Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="74395-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="74395-107">**Buka dengan Explorer** tidak tersedia dalam pengalaman modern untuk pustaka SharePoint.</span><span class="sxs-lookup"><span data-stu-id="74395-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="74395-108">Gunakan **tampilan di file Explorer** .</span><span class="sxs-lookup"><span data-stu-id="74395-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="74395-109">Pilih tampilan **opsi tampilan** \> **di file Explorer**.</span><span class="sxs-lookup"><span data-stu-id="74395-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="74395-110">Tampilan di file Explorer tidak kompatibel dengan Microsoft Edge, Google Chrome, Firefox, dan lainnya.</span><span class="sxs-lookup"><span data-stu-id="74395-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="74395-111">**Tampilkan di file Explorer** hanya tersedia di Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="74395-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="74395-112">Pastikan Layanan WebClient berjalan.</span><span class="sxs-lookup"><span data-stu-id="74395-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="74395-113">Dalam kotak pencarian Windows, ketik jalankan, pilih Jalankan aplikasi desktop, ketikkan Services. MSC, lalu tekan Enter.</span><span class="sxs-lookup"><span data-stu-id="74395-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="74395-114">Gulir ke bawah ke layanan WebClient dan pastikan kolom **status** menampilkan "berjalan."</span><span class="sxs-lookup"><span data-stu-id="74395-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="74395-115">Jika tidak, klik ganda Layanan tersebut, klik **mulai**, lalu klik **OK**.</span><span class="sxs-lookup"><span data-stu-id="74395-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="74395-116">(Anda mungkin harus terlebih dahulu mengaktifkan layanan dengan memilih **manual** atau **otomatis** dalam kotak **tipe startup** .)</span><span class="sxs-lookup"><span data-stu-id="74395-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="74395-117">Membuka pustaka di file Explorer sangat berguna jika Anda perlu menyalin atau memindahkan beberapa file dan folder satu kali, tapi jika Anda ingin bekerja secara teratur di pustaka, kami sarankan menyinkronkannya.</span><span class="sxs-lookup"><span data-stu-id="74395-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="74395-118">Untuk memecahkan masalah yang dibuka di file Explorer, lihat [membuka di Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="74395-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="74395-119">Untuk informasi tentang penyiapan sinkronisasi, lihat [menyinkronkan file SharePoint dengan klien sinkronisasi OneDrive baru](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="74395-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="74395-120">Silakan lihat artikel [cara menggunakan perintah "Buka dengan Explorer" untuk memecahkan masalah di SharePoint online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) untuk informasi selengkapnya.</span><span class="sxs-lookup"><span data-stu-id="74395-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

