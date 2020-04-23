---
title: Memecahkan masalah menggunakan Buka Explorer
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: cb26876d93a110b3b0addd7821206215c783f959
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759695"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="da6e3-102">Memperbaiki masalah saat membuka dengan Explorer</span><span class="sxs-lookup"><span data-stu-id="da6e3-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="da6e3-103">Memperbaiki masalah umum dengan membuka pustaka dokumen di SharePoint atau OneDrive menggunakan perintah **buka dengan Explorer** :</span><span class="sxs-lookup"><span data-stu-id="da6e3-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="da6e3-104">Menggunakan Internet Explorer 10 atau Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="da6e3-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="da6e3-105">**Terbuka dengan Explorer** tidak kompatibel dengan Microsoft Edge, Google Chrome, Firefox dan lain-lain.</span><span class="sxs-lookup"><span data-stu-id="da6e3-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="da6e3-106">**Terbuka dengan Explorer** dinonaktifkan di semua browser kecuali Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="da6e3-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="da6e3-107">**Terbuka dengan Explorer** tidak tersedia dalam pengalaman modern untuk Perpustakaan SharePoint.</span><span class="sxs-lookup"><span data-stu-id="da6e3-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="da6e3-108">Gunakan **tampilan di file Explorer** sebagai gantinya.</span><span class="sxs-lookup"><span data-stu-id="da6e3-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="da6e3-109">Pilih tampilan **opsi** \> tampilan **di file Explorer**.</span><span class="sxs-lookup"><span data-stu-id="da6e3-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="da6e3-110">Lihat di file Explorer tidak kompatibel dengan Microsoft Edge, Google Chrome, Firefox dan lain-lain.</span><span class="sxs-lookup"><span data-stu-id="da6e3-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="da6e3-111">**Lihat di file Explorer** di tersedia hanya di Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="da6e3-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="da6e3-112">Pastikan Layanan WebClient berjalan.</span><span class="sxs-lookup"><span data-stu-id="da6e3-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="da6e3-113">Di kotak pencarian Windows, ketik jalankan, pilih Jalankan aplikasi desktop, ketik Services. MSC, dan kemudian tekan Enter.</span><span class="sxs-lookup"><span data-stu-id="da6e3-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="da6e3-114">Scroll ke bawah ke layanan WebClient dan pastikan kolom **status** menampilkan "Running".</span><span class="sxs-lookup"><span data-stu-id="da6e3-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="da6e3-115">Jika tidak, klik dua kali layanan, klik **mulai**, dan kemudian klik **OK**.</span><span class="sxs-lookup"><span data-stu-id="da6e3-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="da6e3-116">(Anda mungkin perlu terlebih dahulu mengaktifkan layanan dengan memilih salah satu **manual** atau **otomatis** dalam **jenis startup** kotak.)</span><span class="sxs-lookup"><span data-stu-id="da6e3-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="da6e3-117">Membuka perpustakaan di file Explorer sangat berguna jika Anda perlu menyalin atau memindahkan beberapa file dan folder sekali, tetapi jika Anda ingin bekerja secara teratur di Perpustakaan, kami sarankan untuk menyinkronkannya.</span><span class="sxs-lookup"><span data-stu-id="da6e3-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="da6e3-118">Untuk memecahkan masalah pembukaan di file Explorer, lihat [buka di Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="da6e3-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="da6e3-119">Untuk informasi tentang cara menyiapkan sinkronisasi, lihat [menyinkronkan berkas SharePoint dengan klien sinkronisasi OneDrive baru](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="da6e3-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="da6e3-120">Silakan lihat artikel [cara menggunakan perintah "Buka dengan Explorer" untuk memecahkan masalah di SharePoint online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) untuk informasi lebih lanjut.</span><span class="sxs-lookup"><span data-stu-id="da6e3-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

