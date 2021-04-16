---
title: Menggunakan opsi buka kunci sidik jari di Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796680"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="2ecbe-102">Menggunakan opsi buka kunci sidik jari di Windows 10</span><span class="sxs-lookup"><span data-stu-id="2ecbe-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="2ecbe-103">**Mengaktifkan Sidik Jari Windows Hello**</span><span class="sxs-lookup"><span data-stu-id="2ecbe-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="2ecbe-104">Untuk membuka kunci Windows 10 menggunakan sidik jari, Anda perlu menyiapkan Sidik Jari Windows Hello dengan menambahkan (memungkinkan Windows mempelajari cara mengenali) setidaknya satu jari.</span><span class="sxs-lookup"><span data-stu-id="2ecbe-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="2ecbe-105">Masuk ke **Pengaturan > Akun > opsi Masuk (atau** klik di [sini](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="2ecbe-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="2ecbe-106">Opsi masuk yang tersedia akan dicantumkan.</span><span class="sxs-lookup"><span data-stu-id="2ecbe-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="2ecbe-107">Misalnya:</span><span class="sxs-lookup"><span data-stu-id="2ecbe-107">For example:</span></span>

    ![Opsi masuk.](media/sign-in-options.png)

2. <span data-ttu-id="2ecbe-109">Klik atau ketuk **Sidik Jari Windows Hello,** lalu **klik Siapkan.**</span><span class="sxs-lookup"><span data-stu-id="2ecbe-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="2ecbe-110">Di jendela penyiapan Windows Hello, **klik Mulai**.</span><span class="sxs-lookup"><span data-stu-id="2ecbe-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="2ecbe-111">Sensor sidik jari akan aktif, dan Anda akan diminta untuk menempatkan jari di sensor:</span><span class="sxs-lookup"><span data-stu-id="2ecbe-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Sensor sidik jari.](media/fingerprint-sensor.png)

3. <span data-ttu-id="2ecbe-113">Ikuti instruksi, yang akan meminta Anda untuk memindai jari berulang kali.</span><span class="sxs-lookup"><span data-stu-id="2ecbe-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="2ecbe-114">Setelah ini selesai, Anda akan memiliki opsi untuk menambahkan jari lain yang mungkin ingin Anda gunakan untuk masuk.</span><span class="sxs-lookup"><span data-stu-id="2ecbe-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="2ecbe-115">Pada kali berikutnya masuk ke Windows 10, Anda akan memiliki opsi untuk menggunakan sidik jari Anda.</span><span class="sxs-lookup"><span data-stu-id="2ecbe-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="2ecbe-116">**Sidik Jari Windows Hello tidak tersedia sebagai opsi masuk**</span><span class="sxs-lookup"><span data-stu-id="2ecbe-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="2ecbe-117">Jika Sidik Jari Windows Hello tidak diperlihatkan sebagai opsi Masuk **,** artinya Windows tidak mengetahui pembaca/pemindai sidik jari apa pun yang terhubung ke PC Anda, atau bahwa kebijakan sistem mencegah penggunaannya (jika misalnya PC Anda dikelola oleh tempat kerja Anda).</span><span class="sxs-lookup"><span data-stu-id="2ecbe-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="2ecbe-118">Untuk memecahkan masalah:</span><span class="sxs-lookup"><span data-stu-id="2ecbe-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="2ecbe-119">Pilih **tombol** Mulai di Taskbar, lalu cari **Manajer Perangkat.**</span><span class="sxs-lookup"><span data-stu-id="2ecbe-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="2ecbe-120">Klik atau ketuk untuk membuka **Manajer Perangkat.**</span><span class="sxs-lookup"><span data-stu-id="2ecbe-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="2ecbe-121">Di Manajer Perangkat, perluas perangkat Biometrik dengan mengklik chevronnya.</span><span class="sxs-lookup"><span data-stu-id="2ecbe-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Perangkat biometrik.](media/biometric-devices.png)

4. <span data-ttu-id="2ecbe-123">Pemindai sidik jari Anda akan tercantum sebagai perangkat biometrik, seperti pemindai WBDI Synaptics:</span><span class="sxs-lookup"><span data-stu-id="2ecbe-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Perangkat biometrik.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="2ecbe-125">Jika pemindai sidik jari Anda tidak terlihat, dan pemindai terintegrasi dengan PC Anda, masuk ke situs web pabrikan PC.</span><span class="sxs-lookup"><span data-stu-id="2ecbe-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="2ecbe-126">Di bagian dukungan teknis untuk model PC Anda, cari driver Windows 10 untuk pemindai yang dapat diinstal.</span><span class="sxs-lookup"><span data-stu-id="2ecbe-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="2ecbe-127">Jika pemindai terpisah dari PC (dilampirkan melalui USB), masuk ke situs web produsen pemindai untuk menemukan dan menginstal perangkat lunak driver perangkat Windows 10 untuk model pemindai yang Anda miliki.</span><span class="sxs-lookup"><span data-stu-id="2ecbe-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
