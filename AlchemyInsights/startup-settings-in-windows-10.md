---
title: Pengaturan startup di Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: e49faca66785c6611dda702a381c39cdb10884f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751138"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="91469-102">Pengaturan startup di Windows 10</span><span class="sxs-lookup"><span data-stu-id="91469-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="91469-103">**Mengubah aplikasi yang berjalan secara otomatis pada saat startup**</span><span class="sxs-lookup"><span data-stu-id="91469-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="91469-104">Masuk ke [pengaturan > aplikasi > mulai](ms-settings:startupapps?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="91469-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="91469-105">Pastikan semua aplikasi yang ingin Anda **jalankan pada startup diaktifkan.**</span><span class="sxs-lookup"><span data-stu-id="91469-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="91469-106">**Menambahkan aplikasi untuk dijalankan secara otomatis saat memulai**</span><span class="sxs-lookup"><span data-stu-id="91469-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="91469-107">Klik atau ketuk **mulai** dan temukan aplikasi yang ingin Anda jalankan pada startup.</span><span class="sxs-lookup"><span data-stu-id="91469-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="91469-108">Klik kanan aplikasi, klik **lainnya**, lalu klik **buka lokasi file**.</span><span class="sxs-lookup"><span data-stu-id="91469-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="91469-109">Ini akan membuka lokasi tempat pintasan ke aplikasi disimpan.</span><span class="sxs-lookup"><span data-stu-id="91469-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="91469-110">Jika tidak ada opsi untuk lokasi file yang terbuka, itu berarti aplikasi tidak dapat dijalankan pada startup.</span><span class="sxs-lookup"><span data-stu-id="91469-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="91469-111">Dengan lokasi file terbuka, tekan **tombol logo Windows + R**, ketikkan **Shell: startup**, lalu klik **OK**.</span><span class="sxs-lookup"><span data-stu-id="91469-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="91469-112">Ini akan membuka folder startup.</span><span class="sxs-lookup"><span data-stu-id="91469-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="91469-113">Salin dan tempelkan pintasan ke aplikasi dari lokasi file ke folder startup.</span><span class="sxs-lookup"><span data-stu-id="91469-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="91469-114">**Opsi startup tingkat lanjut (termasuk mode aman, pengaturan UEFI, dan booting dari perangkat lain)**</span><span class="sxs-lookup"><span data-stu-id="91469-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="91469-115">Simpan pekerjaan Anda dan tutup setiap dokumen yang terbuka, karena langkah-langkah ini akan memulai ulang PC Anda.</span><span class="sxs-lookup"><span data-stu-id="91469-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="91469-116">Buka [pengaturan > perbarui & keamanan > pemulihan](ms-settings:recovery?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="91469-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="91469-117">Di bawah **startup tingkat lanjut**, klik **mulai ulang sekarang**.</span><span class="sxs-lookup"><span data-stu-id="91469-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="91469-118">Setelah PC dimulai ulang ke layar pilih opsi:</span><span class="sxs-lookup"><span data-stu-id="91469-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="91469-119">Untuk boot dari perangkat seperti drive USB, klik **Gunakan perangkat**.</span><span class="sxs-lookup"><span data-stu-id="91469-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="91469-120">Untuk memasukkan pengaturan UEFI (terkadang disebut penyetelan BIOS), klik **pemecahan masalah > opsi tingkat lanjut > UEFI pengaturan firmware**.</span><span class="sxs-lookup"><span data-stu-id="91469-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="91469-121">Untuk memasukkan mode aman atau mengubah pengaturan startup tingkat lanjut, klik **pemecahan masalah > opsi tingkat lanjut > pengaturan startup**, lalu klik **mulai ulang**.</span><span class="sxs-lookup"><span data-stu-id="91469-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="91469-122">Anda mungkin diminta untuk memasukkan [kunci pemulihan BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span><span class="sxs-lookup"><span data-stu-id="91469-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="91469-123">Setelah PC dimulai ulang lagi, klik Pengaturan mulai yang ingin Anda gunakan.</span><span class="sxs-lookup"><span data-stu-id="91469-123">After your PC restarts again, click the startup setting you want to use.</span></span>