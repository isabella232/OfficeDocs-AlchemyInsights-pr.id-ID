---
title: File membuka hanya-baca
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6a828f8d-ff31-40a7-b701-b2339e771817
ms.openlocfilehash: 4c774864a03b7dbc099f64b7906fa4a0bc26c63c
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525744"
---
# <a name="file-open-read-only"></a><span data-ttu-id="8ced9-102">File membuka hanya-baca</span><span class="sxs-lookup"><span data-stu-id="8ced9-102">File open read-only</span></span>

<span data-ttu-id="8ced9-103">Anda mungkin menemukan bahwa ketika Anda membuka file, mereka membuka sebagai baca-saja.</span><span class="sxs-lookup"><span data-stu-id="8ced9-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="8ced9-104">Dalam beberapa kasus, ini adalah untuk keamanan tambahan, seperti ketika Anda membuka file dari internet, dan lain kali, itu bisa karena pengaturan yang dapat diubah.</span><span class="sxs-lookup"><span data-stu-id="8ced9-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="8ced9-105">Berikut adalah beberapa skenario di mana sebuah file terbuka hanya-baca dan beberapa langkah yang dapat Anda ambil untuk mengubah itu.</span><span class="sxs-lookup"><span data-stu-id="8ced9-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="8ced9-106">**My antivirus menyebabkan mereka untuk membuka hanya-baca**</span><span class="sxs-lookup"><span data-stu-id="8ced9-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="8ced9-107">Beberapa program antivirus dapat melindungi Anda dari file yang berpotensi tidak aman dengan membuka mereka hanya-baca.</span><span class="sxs-lookup"><span data-stu-id="8ced9-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="8ced9-108">Anda mungkin perlu memeriksa dengan penyedia antivirus untuk belajar bagaimana untuk menyesuaikan setelan ini.</span><span class="sxs-lookup"><span data-stu-id="8ced9-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="8ced9-109">BitDefender, misalnya, memiliki kandungan menambahkan aplikasi pengecualian di sini: [Bagaimana menambahkan aplikasi atau proses pengecualian di Bitdefender kontrol pusat](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span><span class="sxs-lookup"><span data-stu-id="8ced9-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span></span>
  
 <span data-ttu-id="8ced9-110">**File properti diatur untuk hanya-baca?**</span><span class="sxs-lookup"><span data-stu-id="8ced9-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="8ced9-111">Anda dapat memeriksa file properti dengan mengklik kanan pada file dan memilih properti.</span><span class="sxs-lookup"><span data-stu-id="8ced9-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="8ced9-112">Jika atribut hanya-baca di-cek, Anda dapat Hapus centang dan klik OK.</span><span class="sxs-lookup"><span data-stu-id="8ced9-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="8ced9-113">**Konten yang dilindungi pemandangan**</span><span class="sxs-lookup"><span data-stu-id="8ced9-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="8ced9-114">File dari Internet dan dari lokasi lain berpotensi tidak aman dapat berisi virus, cacing, atau malware yang dapat membahayakan komputer jenis lain.</span><span class="sxs-lookup"><span data-stu-id="8ced9-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="8ced9-115">Hal ini juga sering terjadi dengan lampiran email atau berkas yang Anda unduh.</span><span class="sxs-lookup"><span data-stu-id="8ced9-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="8ced9-116">Untuk membantu melindungi komputer Anda, file dari lokasi ini berpotensi tidak aman dibuka dalam pandangan dilindungi.</span><span class="sxs-lookup"><span data-stu-id="8ced9-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="8ced9-117">Dengan menggunakan View dilindungi, Anda dapat membaca file dan melihat isinya sementara mengurangi resiko.</span><span class="sxs-lookup"><span data-stu-id="8ced9-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="8ced9-118">Untuk informasi lebih lanjut lihat dilindungi dan bagaimana untuk mengubah pengaturan, lihat artikel ini: [apa itu dilindungi View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="8ced9-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="8ced9-119">**Apakah OneDrive penuh?**</span><span class="sxs-lookup"><span data-stu-id="8ced9-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="8ced9-120">Jika berkas tersebut disimpan pada OneDrive dan ruang penyimpanan OneDrive Anda penuh, Anda akan mampu menyimpan dokumen sampai Anda berada di bawah Anda ruang yang diberikan.</span><span class="sxs-lookup"><span data-stu-id="8ced9-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="8ced9-121">Anda dapat memeriksa Anda ruang kosong pada OneDrive dengan mengklik ikon OneDrive di pusat pemberitahuan dan memilih Kelola penyimpanan, atau Anda dapat pergi ke [http://onedrive.live.com](http://onedrive.live.com), masuk, dan perhatikan jumlah ruang yang digunakan di bawah kiri layar.</span><span class="sxs-lookup"><span data-stu-id="8ced9-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [http://onedrive.live.com](http://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="8ced9-122">**Kantor diaktifkan?**</span><span class="sxs-lookup"><span data-stu-id="8ced9-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="8ced9-123">Jika kantor tidak diaktifkan, atau jika langganan Anda telah kedaluwarsa, Anda bisa hanya-baca dikurangi fungsi mode.</span><span class="sxs-lookup"><span data-stu-id="8ced9-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="8ced9-124">Untuk selengkapnya tentang cara mengaktifkan kantor, lihat: [produk berlisensi dan aktivasi kesalahan di kantor](https://support.office.com/article/unlicensed-product-and-activation-errors-in-office-0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="8ced9-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/unlicensed-product-and-activation-errors-in-office-0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="8ced9-125">**Jika semuanya gagal...**</span><span class="sxs-lookup"><span data-stu-id="8ced9-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="8ced9-126">Coba mulai ulang komputer</span><span class="sxs-lookup"><span data-stu-id="8ced9-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="8ced9-127">Menginstal pemutakhiran Office</span><span class="sxs-lookup"><span data-stu-id="8ced9-127">Install Office updates</span></span>
    
- <span data-ttu-id="8ced9-128">Melakukan perbaikan kantor Online</span><span class="sxs-lookup"><span data-stu-id="8ced9-128">Perform an Online repair of Office</span></span>
    

