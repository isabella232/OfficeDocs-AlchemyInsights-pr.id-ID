---
title: File Buka baca-saja
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 2fdb4f048c2bee022a49c2cca2ce9770f42a87a2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745589"
---
# <a name="file-open-read-only"></a><span data-ttu-id="eb451-102">File Buka baca-saja</span><span class="sxs-lookup"><span data-stu-id="eb451-102">File open read-only</span></span>

<span data-ttu-id="eb451-103">Anda mungkin menemukan bahwa saat Anda membuka file, mereka membuka sebagai baca-saja.</span><span class="sxs-lookup"><span data-stu-id="eb451-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="eb451-104">Dalam beberapa kasus, ini adalah untuk keamanan tambahan, seperti saat Anda membuka file dari internet, dan waktu lainnya, ini bisa disebabkan pengaturan yang bisa diubah.</span><span class="sxs-lookup"><span data-stu-id="eb451-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="eb451-105">Berikut adalah beberapa skenario di mana file membuka baca-saja dan beberapa langkah yang bisa Anda lakukan untuk mengubahnya.</span><span class="sxs-lookup"><span data-stu-id="eb451-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="eb451-106">**Antivirus saya menyebabkan mereka membuka baca-saja**</span><span class="sxs-lookup"><span data-stu-id="eb451-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="eb451-107">Beberapa program antivirus mungkin memproteksi Anda dari file yang berpotensi tidak aman dengan membukanya baca-saja.</span><span class="sxs-lookup"><span data-stu-id="eb451-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="eb451-108">Anda mungkin perlu memeriksa penyedia antivirus untuk mempelajari cara menyesuaikan pengaturan ini.</span><span class="sxs-lookup"><span data-stu-id="eb451-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="eb451-109">BitDefender, misalnya, memiliki konten untuk menambahkan pengecualian aplikasi di sini: [cara menambahkan pengecualian aplikasi atau proses di pusat kontrol BitDefender](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="eb451-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="eb451-110">**Apakah properti file diatur ke baca-saja?**</span><span class="sxs-lookup"><span data-stu-id="eb451-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="eb451-111">Anda dapat memeriksa properti file dengan mengklik kanan file dan memilih properti.</span><span class="sxs-lookup"><span data-stu-id="eb451-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="eb451-112">Jika atribut baca-saja dicentang, Anda bisa menghapus centang dan klik OK.</span><span class="sxs-lookup"><span data-stu-id="eb451-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="eb451-113">**Konten dalam tampilan terproteksi**</span><span class="sxs-lookup"><span data-stu-id="eb451-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="eb451-114">File dari internet dan dari lokasi yang berpotensi tidak aman lainnya dapat berisi virus, worm, atau jenis malware lainnya yang bisa membahayakan komputer Anda.</span><span class="sxs-lookup"><span data-stu-id="eb451-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="eb451-115">Ini juga sering terjadi pada lampiran email atau file yang telah Anda unduh.</span><span class="sxs-lookup"><span data-stu-id="eb451-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="eb451-116">Untuk membantu melindungi komputer Anda, file dari lokasi yang berpotensi tidak aman dibuka dalam tampilan terproteksi.</span><span class="sxs-lookup"><span data-stu-id="eb451-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="eb451-117">Dengan menggunakan tampilan terproteksi, Anda bisa membaca file dan melihat kontennya sambil mengurangi risiko.</span><span class="sxs-lookup"><span data-stu-id="eb451-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="eb451-118">Untuk informasi selengkapnya tentang tampilan terproteksi dan cara mengubah pengaturan, lihat artikel ini: [apa itu tampilan terproteksi?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="eb451-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="eb451-119">**Apakah OneDrive sudah penuh?**</span><span class="sxs-lookup"><span data-stu-id="eb451-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="eb451-120">Jika file disimpan di OneDrive dan ruang penyimpanan OneDrive Anda penuh, Anda tidak akan bisa menyimpan dokumen hingga Anda berada di bawah ruang yang dialokasikan.</span><span class="sxs-lookup"><span data-stu-id="eb451-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="eb451-121">Anda bisa memeriksa ruang kosong Anda di OneDrive dengan mengklik ikon OneDrive di pusat pemberitahuan dan memilih Kelola penyimpanan, atau Anda bisa masuk ke [https://onedrive.live.com](https://onedrive.live.com) , masuk, dan catat jumlah ruang yang digunakan di bagian kiri bawah layar.</span><span class="sxs-lookup"><span data-stu-id="eb451-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="eb451-122">**Apakah Office diaktifkan?**</span><span class="sxs-lookup"><span data-stu-id="eb451-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="eb451-123">Jika Office tidak diaktifkan, atau jika langganan Anda telah kedaluwarsa, Anda mungkin berada dalam mode fungsionalitas yang dikurangi baca-saja.</span><span class="sxs-lookup"><span data-stu-id="eb451-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="eb451-124">Untuk informasi tentang cara mengaktifkan Office, lihat: [produk tanpa lisensi dan kesalahan aktivasi di Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="eb451-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="eb451-125">**Jika semuanya gagal...**</span><span class="sxs-lookup"><span data-stu-id="eb451-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="eb451-126">Coba mulai ulang komputer</span><span class="sxs-lookup"><span data-stu-id="eb451-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="eb451-127">Menginstal pembaruan Office</span><span class="sxs-lookup"><span data-stu-id="eb451-127">Install Office updates</span></span>
    
- <span data-ttu-id="eb451-128">Menjalankan perbaikan online Office</span><span class="sxs-lookup"><span data-stu-id="eb451-128">Perform an Online repair of Office</span></span>
    

