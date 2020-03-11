---
title: Gunakan opsi Buka kunci sidik jari di Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 8a5059c722c306ad79811140062cec7f52f31766
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588319"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="93131-102">Gunakan opsi Buka kunci sidik jari di Windows 10</span><span class="sxs-lookup"><span data-stu-id="93131-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="93131-103">**Mengaktifkan Windows Hello Fingerprint**</span><span class="sxs-lookup"><span data-stu-id="93131-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="93131-104">Untuk membuka Windows 10 menggunakan sidik jari Anda, Anda perlu mengatur Windows Hello Fingerprint dengan menambahkan (membiarkan Windows belajar mengenali) setidaknya satu jari.</span><span class="sxs-lookup"><span data-stu-id="93131-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="93131-105">Buka **pengaturan > akun > opsi masuk** (atau klik [di sini](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="93131-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="93131-106">Opsi masuk yang tersedia akan dicantumkan.</span><span class="sxs-lookup"><span data-stu-id="93131-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="93131-107">Misalnya:</span><span class="sxs-lookup"><span data-stu-id="93131-107">For example:</span></span>

    ![Opsi masuk.](media/sign-in-options.png)

2. <span data-ttu-id="93131-109">Klik atau ketuk **Windows Halo sidik jari**, lalu klik **Siapkan**.</span><span class="sxs-lookup"><span data-stu-id="93131-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="93131-110">Di jendela penyiapan Windows Hello, klik **mulai**.</span><span class="sxs-lookup"><span data-stu-id="93131-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="93131-111">Sensor sidik jari akan aktif, dan Anda akan diminta untuk menempatkan jari Anda pada sensor:</span><span class="sxs-lookup"><span data-stu-id="93131-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Sensor sidik jari.](media/fingerprint-sensor.png)

3. <span data-ttu-id="93131-113">Ikuti petunjuk yang akan meminta Anda untuk memindai jari secara berulang-ulang.</span><span class="sxs-lookup"><span data-stu-id="93131-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="93131-114">Setelah ini selesai, Anda akan memiliki opsi untuk menambahkan jari lain yang mungkin ingin Anda gunakan untuk masuk.</span><span class="sxs-lookup"><span data-stu-id="93131-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="93131-115">Lain kali Anda masuk ke Windows 10, Anda akan memiliki pilihan untuk menggunakan sidik jari Anda untuk melakukannya.</span><span class="sxs-lookup"><span data-stu-id="93131-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="93131-116">**Windows Halo sidik jari tidak tersedia sebagai Opsi masuk**</span><span class="sxs-lookup"><span data-stu-id="93131-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="93131-117">Jika Windows Halo sidik jari tidak ditampilkan sebagai pilihan dalam **sign-in pilihan**, itu berarti Windows tidak menyadari setiap sidik jari pembaca/scanner MELEKAT pada PC Anda, atau bahwa kebijakan sistem mencegah penggunaannya (jika misalnya PC Anda dikelola oleh tempat kerja Anda).</span><span class="sxs-lookup"><span data-stu-id="93131-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="93131-118">Untuk memecahkan masalah:</span><span class="sxs-lookup"><span data-stu-id="93131-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="93131-119">Pilih tombol **mulai** di taskbar dan Cari **Device Manager**.</span><span class="sxs-lookup"><span data-stu-id="93131-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="93131-120">Klik atau ketuk untuk membuka **pengelola perangkat**.</span><span class="sxs-lookup"><span data-stu-id="93131-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="93131-121">Pada pengelola perangkat, Perluas perangkat biometrik dengan mengeklik Chevron-nya.</span><span class="sxs-lookup"><span data-stu-id="93131-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Perangkat biometrik.](media/biometric-devices.png)

4. <span data-ttu-id="93131-123">Pemindai sidik jari Anda harus terdaftar sebagai perangkat biometrik, seperti pemindai WBDI Synaptics:</span><span class="sxs-lookup"><span data-stu-id="93131-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Perangkat biometrik.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="93131-125">Jika pemindai sidik jari Anda tidak ditampilkan, dan pemindai diintegrasikan ke dalam PC Anda, buka situs web produsen PC.</span><span class="sxs-lookup"><span data-stu-id="93131-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="93131-126">Di bagian dukungan teknis untuk model PC Anda, Cari Driver Windows 10 untuk pemindai yang dapat Anda instal.</span><span class="sxs-lookup"><span data-stu-id="93131-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="93131-127">Jika pemindai terpisah dari PC (terpasang melalui USB), buka situs web produsen pemindai untuk menemukan dan menginstal perangkat lunak pengandar perangkat Windows 10 untuk model pemindai yang Anda miliki.</span><span class="sxs-lookup"><span data-stu-id="93131-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
