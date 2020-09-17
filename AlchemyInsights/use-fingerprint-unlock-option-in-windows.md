---
title: Menggunakan opsi Unlock Fingerprint di Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795247"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="44115-102">Menggunakan opsi Unlock Fingerprint di Windows 10</span><span class="sxs-lookup"><span data-stu-id="44115-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="44115-103">**Mengaktifkan sidik jari Windows Hello**</span><span class="sxs-lookup"><span data-stu-id="44115-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="44115-104">Untuk membuka kunci Windows 10 menggunakan sidik jari, Anda perlu menyetel sidik jari Windows Hello dengan menambahkan (membiarkan jendela mempelajari cara mengenali) setidaknya satu jari.</span><span class="sxs-lookup"><span data-stu-id="44115-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="44115-105">Masuk ke **pengaturan > akun > opsi masuk** (atau klik [di sini](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="44115-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="44115-106">Opsi masuk yang tersedia akan dicantumkan.</span><span class="sxs-lookup"><span data-stu-id="44115-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="44115-107">Misalnya:</span><span class="sxs-lookup"><span data-stu-id="44115-107">For example:</span></span>

    ![Opsi masuk.](media/sign-in-options.png)

2. <span data-ttu-id="44115-109">Klik atau ketuk **sidik jari Windows Hello**, lalu klik **Siapkan**.</span><span class="sxs-lookup"><span data-stu-id="44115-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="44115-110">Di jendela penyetelan Windows Hello, klik **mulai**.</span><span class="sxs-lookup"><span data-stu-id="44115-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="44115-111">Sensor sidik jari akan aktif, dan Anda akan diminta untuk meletakkan jari Anda pada sensor:</span><span class="sxs-lookup"><span data-stu-id="44115-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Sensor sidik jari.](media/fingerprint-sensor.png)

3. <span data-ttu-id="44115-113">Ikuti instruksi, yang akan meminta Anda untuk berulang kali memindai jari Anda.</span><span class="sxs-lookup"><span data-stu-id="44115-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="44115-114">Setelah selesai, Anda akan memiliki opsi untuk menambahkan jari lain yang mungkin ingin Anda gunakan untuk masuk.</span><span class="sxs-lookup"><span data-stu-id="44115-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="44115-115">Saat berikutnya Anda masuk ke Windows 10, Anda akan memiliki opsi untuk menggunakan sidik jari Anda untuk melakukannya.</span><span class="sxs-lookup"><span data-stu-id="44115-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="44115-116">**Sidik jari Windows Hello tidak tersedia sebagai Opsi masuk**</span><span class="sxs-lookup"><span data-stu-id="44115-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="44115-117">Jika sidik jari Windows Hello tidak diperlihatkan sebagai Opsi **masuk**, artinya Windows tidak mengetahui pembaca/pemindai sidik jari apa pun yang MELEKAT pada PC Anda, atau bahwa kebijakan sistem mencegah penggunaannya (jika misalnya PC dikelola oleh tempat kerja Anda).</span><span class="sxs-lookup"><span data-stu-id="44115-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="44115-118">Untuk memecahkan masalah:</span><span class="sxs-lookup"><span data-stu-id="44115-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="44115-119">Pilih tombol **mulai** di taskbar dan Cari **manajer perangkat**.</span><span class="sxs-lookup"><span data-stu-id="44115-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="44115-120">Klik atau ketuk untuk membuka **manajer perangkat**.</span><span class="sxs-lookup"><span data-stu-id="44115-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="44115-121">Di manajer perangkat, Perluas perangkat biometrik dengan mengklik Chevron.</span><span class="sxs-lookup"><span data-stu-id="44115-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Perangkat biometrik.](media/biometric-devices.png)

4. <span data-ttu-id="44115-123">Pemindai sidik jari Anda harus dicantumkan sebagai perangkat biometrik, seperti pemindai Synaptics WBDI:</span><span class="sxs-lookup"><span data-stu-id="44115-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Perangkat biometrik.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="44115-125">Jika pemindai sidik jari tidak diperlihatkan, dan pemindai diintegrasikan ke PC Anda, buka situs web produsen PC.</span><span class="sxs-lookup"><span data-stu-id="44115-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="44115-126">Di bagian dukungan teknis untuk model PC Anda, Cari Driver Windows 10 untuk pemindai yang bisa Anda instal.</span><span class="sxs-lookup"><span data-stu-id="44115-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="44115-127">Jika pemindai terpisah dari PC (dilampirkan melalui USB), buka situs web pabrikan pemindai untuk menemukan dan menginstal perangkat lunak driver perangkat Windows 10 untuk model pemindai yang Anda miliki.</span><span class="sxs-lookup"><span data-stu-id="44115-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
