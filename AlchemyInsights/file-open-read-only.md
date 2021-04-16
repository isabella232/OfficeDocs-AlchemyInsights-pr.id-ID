---
title: File terbuka sebagai baca-saja
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: e478572ea82e5ea11bac9fd7eacafb833253235d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813187"
---
# <a name="file-open-read-only"></a><span data-ttu-id="6926f-102">File terbuka sebagai baca-saja</span><span class="sxs-lookup"><span data-stu-id="6926f-102">File open read-only</span></span>

<span data-ttu-id="6926f-103">Ketika membuka file, Anda mungkin meningka bahwa file terbuka sebagai baca-saja.</span><span class="sxs-lookup"><span data-stu-id="6926f-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="6926f-104">Dalam beberapa kasus, hal ini dilakukan untuk keamanan tambahan, seperti ketika Anda membuka file dari internet, atau mungkin dikarenakan pengaturan yang dapat diubah.</span><span class="sxs-lookup"><span data-stu-id="6926f-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="6926f-105">Berikut adalah beberapa skenario ketika file terbuka sebagai baca-saja dan langkah yang dapat dilakukan untuk mengubahnya.</span><span class="sxs-lookup"><span data-stu-id="6926f-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="6926f-106">**Antivirus saya menyebabkan file terbuka sebagai baca-saja**</span><span class="sxs-lookup"><span data-stu-id="6926f-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="6926f-107">Beberapa program antivirus mungkin melindungi Anda dari file yang berpotensi tidak aman dengan membukanya sebagai baca-saja.</span><span class="sxs-lookup"><span data-stu-id="6926f-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="6926f-108">Anda mungkin perlu memeriksa penyedia antivirus untuk mempelajari cara menyesuaikan pengaturan ini.</span><span class="sxs-lookup"><span data-stu-id="6926f-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="6926f-109">BitDefender, misalnya, memiliki konten tentang menambahkan pengecualian aplikasi berikut ini: Cara menambahkan pengecualian proses atau aplikasi di [Pusat Kontrol Bitdefender.](https://aka.ms/AA6098i)</span><span class="sxs-lookup"><span data-stu-id="6926f-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="6926f-110">**Apakah properti file diatur menjadi baca-saja?**</span><span class="sxs-lookup"><span data-stu-id="6926f-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="6926f-111">Anda dapat memeriksa properti file dengan mengklik kanan file dan memilih Properti.</span><span class="sxs-lookup"><span data-stu-id="6926f-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="6926f-112">Jika atribut Baca-saja dicentang, Anda dapat menghapus centang tersebut dan mengklik OK.</span><span class="sxs-lookup"><span data-stu-id="6926f-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="6926f-113">**Konten berada dalam tampilan terproteksi**</span><span class="sxs-lookup"><span data-stu-id="6926f-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="6926f-114">File dari internet dan lokasi lain yang berpotensi tidak aman dapat berisi virus, worm, atau malware jenis lain yang dapat merusak komputer.</span><span class="sxs-lookup"><span data-stu-id="6926f-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="6926f-115">Hal ini biasanya juga terjadi dengan lampiran email atau file yang diunduh.</span><span class="sxs-lookup"><span data-stu-id="6926f-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="6926f-116">Untuk membantu melindungi komputer Anda, file dari lokasi yang berpotensi tidak aman ini dibuka dalam Tampilan Terproteksi.</span><span class="sxs-lookup"><span data-stu-id="6926f-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="6926f-117">Dengan Tampilan Terproteksi, Anda dapat membaca file dan melihat kontennya sekaligus mengurangi risiko.</span><span class="sxs-lookup"><span data-stu-id="6926f-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="6926f-118">Untuk informasi selengkapnya tentang tampilan Terproteksi dan cara mengubah pengaturan, lihat artikel ini: [Apa yang itu Tampilan Terproteksi?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="6926f-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="6926f-119">**Apakah OneDrive penuh?**</span><span class="sxs-lookup"><span data-stu-id="6926f-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="6926f-120">Jika file disimpan di OneDrive, dan OneDrive penuh, Anda tidak akan dapat menyimpan dokumen hingga tersedia ruang penyimpanan di bawah batas yang diberikan.</span><span class="sxs-lookup"><span data-stu-id="6926f-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="6926f-121">Anda dapat memeriksa ruang yang tersedia di OneDrive dengan mengklik ikon OneDrive di pusat pemberitahuan dan memilih Kelola penyimpanan, atau masuk ke , masuk, lalu catat jumlah ruang yang digunakan di bagian kiri bawah [https://onedrive.live.com](https://onedrive.live.com) layar.</span><span class="sxs-lookup"><span data-stu-id="6926f-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="6926f-122">**Apakah Office diaktifkan?**</span><span class="sxs-lookup"><span data-stu-id="6926f-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="6926f-123">Jika Office tidak diaktifkan, atau jika langganan telah kedaluwarsa, Anda hanya dapat menggunakan Mode Fungsionalitas Berkurang secara baca-saja.</span><span class="sxs-lookup"><span data-stu-id="6926f-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="6926f-124">Untuk informasi tentang cara mengaktifkan Office, lihat: [Produk Tanpa Lisensi dan kesalahan aktivasi di Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="6926f-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="6926f-125">**Jika semuanya gagal...**</span><span class="sxs-lookup"><span data-stu-id="6926f-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="6926f-126">Coba mulai ulang komputer</span><span class="sxs-lookup"><span data-stu-id="6926f-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="6926f-127">Menginstal pembaruan Office</span><span class="sxs-lookup"><span data-stu-id="6926f-127">Install Office updates</span></span>
    
- <span data-ttu-id="6926f-128">Jalankan Perbaikan online Office</span><span class="sxs-lookup"><span data-stu-id="6926f-128">Perform an Online repair of Office</span></span>
    

