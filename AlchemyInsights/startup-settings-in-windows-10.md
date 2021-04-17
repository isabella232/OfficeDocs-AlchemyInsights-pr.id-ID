---
title: Pengaturan mulai di Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: 6dfae58a398db088ba00d9c2ea9788bab929ccc1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51828155"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="ec6b2-102">Pengaturan mulai di Windows 10</span><span class="sxs-lookup"><span data-stu-id="ec6b2-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="ec6b2-103">**Mengubah aplikasi mana yang berjalan secara otomatis saat startup**</span><span class="sxs-lookup"><span data-stu-id="ec6b2-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="ec6b2-104">Masuk ke [Pengaturan > Aplikasi > Mulai](ms-settings:startupapps?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="ec6b2-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="ec6b2-105">Pastikan setiap aplikasi yang ingin Anda jalankan saat startup diaktifkan **ke On**.</span><span class="sxs-lookup"><span data-stu-id="ec6b2-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="ec6b2-106">**Tambahkan aplikasi untuk berjalan secara otomatis saat startup**</span><span class="sxs-lookup"><span data-stu-id="ec6b2-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="ec6b2-107">Klik atau ketuk **Mulai** dan temukan aplikasi yang ingin Anda jalankan saat memulai.</span><span class="sxs-lookup"><span data-stu-id="ec6b2-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="ec6b2-108">Klik kanan aplikasi, klik **Lainnya**, lalu klik **Buka lokasi file.**</span><span class="sxs-lookup"><span data-stu-id="ec6b2-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="ec6b2-109">Tindakan ini akan membuka lokasi tempat pintasan ke aplikasi disimpan.</span><span class="sxs-lookup"><span data-stu-id="ec6b2-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="ec6b2-110">Jika tidak ada opsi untuk Buka lokasi file, artinya aplikasi tidak dapat berjalan saat startup.</span><span class="sxs-lookup"><span data-stu-id="ec6b2-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="ec6b2-111">Dengan lokasi file yang terbuka, tekan tombol **logo Windows + R,** ketik **shell:startup,** lalu klik **OK.**</span><span class="sxs-lookup"><span data-stu-id="ec6b2-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="ec6b2-112">Ini membuka folder Startup.</span><span class="sxs-lookup"><span data-stu-id="ec6b2-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="ec6b2-113">Salin dan tempel pintasan ke aplikasi dari lokasi file ke folder Startup.</span><span class="sxs-lookup"><span data-stu-id="ec6b2-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="ec6b2-114">**Opsi mulai tingkat lanjut (termasuk Mode Aman, pengaturan UEFI, dan booting dari perangkat lain)**</span><span class="sxs-lookup"><span data-stu-id="ec6b2-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="ec6b2-115">Simpan pekerjaan dan tutup dokumen apa pun yang terbuka, karena langkah-langkah ini akan menghidupkan ulang PC Anda.</span><span class="sxs-lookup"><span data-stu-id="ec6b2-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="ec6b2-116">Masuk ke [Pengaturan > Pembaruan & Pemulihan > Anda.](ms-settings:recovery?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="ec6b2-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="ec6b2-117">Di **bawah Mulai ulang** tingkat lanjut, klik Mulai ulang **sekarang.**</span><span class="sxs-lookup"><span data-stu-id="ec6b2-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="ec6b2-118">Setelah PC dihidupkan ulang ke layar Pilih opsi:</span><span class="sxs-lookup"><span data-stu-id="ec6b2-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="ec6b2-119">Untuk melakukan boot dari perangkat seperti drive USB, **klik Gunakan perangkat**.</span><span class="sxs-lookup"><span data-stu-id="ec6b2-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="ec6b2-120">Untuk memasukkan pengaturan UEFI (kadang disebut penyetelan EFE), klik **Pecahkan > Tingkat Lanjut > Pengaturan Firmware UEFI.**</span><span class="sxs-lookup"><span data-stu-id="ec6b2-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="ec6b2-121">Untuk masuk ke Mode Aman atau mengubah pengaturan mulai tingkat lanjut, klik Memecahkan > Opsi **tingkat lanjut > Pengaturan Mulai,** lalu klik Mulai **Ulang.**</span><span class="sxs-lookup"><span data-stu-id="ec6b2-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="ec6b2-122">Anda mungkin diminta untuk memasukkan kunci [pemulihan BitLocker Anda.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key)</span><span class="sxs-lookup"><span data-stu-id="ec6b2-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="ec6b2-123">Setelah PC Anda dihidupkan ulang lagi, klik pengaturan mulai yang ingin Anda gunakan.</span><span class="sxs-lookup"><span data-stu-id="ec6b2-123">After your PC restarts again, click the startup setting you want to use.</span></span>