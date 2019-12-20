---
title: Memecahkan masalah audio di Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3476"
- "9001463"
ms.openlocfilehash: 46b23f97c2e682258224dc95e7a76b1201991828
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796187"
---
# <a name="troubleshooting-audio-problems-in-windows-10"></a><span data-ttu-id="4a9ae-102">Pemecahan masalah audio di Windows 10</span><span class="sxs-lookup"><span data-stu-id="4a9ae-102">Troubleshooting audio problems in Windows 10</span></span>

<span data-ttu-id="4a9ae-103">**Jalankan pemecah masalah audio**</span><span class="sxs-lookup"><span data-stu-id="4a9ae-103">**Run the audio troubleshooter**</span></span>

<span data-ttu-id="4a9ae-104">Pemecah masalah audio mungkin dapat memperbaiki permasalahan audio secara otomatis:</span><span class="sxs-lookup"><span data-stu-id="4a9ae-104">The audio troubleshooter might be able to fix the audio problems automatically:</span></span> 

1. <span data-ttu-id="4a9ae-105">Pilih **mulai**, ketik **pemecahan masalah**, dan kemudian pilih **pemecahan masalah** dari daftar hasil.</span><span class="sxs-lookup"><span data-stu-id="4a9ae-105">Select **Start**, type **troubleshoot**, and then select **Troubleshoot** from the list of results.</span></span> 
2. <span data-ttu-id="4a9ae-106">Pilih **Mainkan audio** > **menjalankan pemecah masalah**.</span><span class="sxs-lookup"><span data-stu-id="4a9ae-106">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="4a9ae-107">**Periksa kabel, volume, speaker, dan headphone**</span><span class="sxs-lookup"><span data-stu-id="4a9ae-107">**Check cables, volume, speakers, and headphones**</span></span>

- <span data-ttu-id="4a9ae-108">Periksa koneksi speaker dan headphone Anda untuk kabel longgar, dan pastikan mereka terhubung ke Jack yang benar.</span><span class="sxs-lookup"><span data-stu-id="4a9ae-108">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>
- <span data-ttu-id="4a9ae-109">Periksa kekuatan dan tingkat volume, dan mencoba mengubah semua kontrol volume atas.</span><span class="sxs-lookup"><span data-stu-id="4a9ae-109">Check your power and volume levels, and try turning all the volume controls up.</span></span>
- <span data-ttu-id="4a9ae-110">Beberapa pembicara dan aplikasi memiliki kontrol volume mereka sendiri, dan Anda mungkin harus memeriksa mereka semua untuk memastikan mereka berada di tingkat yang tepat.</span><span class="sxs-lookup"><span data-stu-id="4a9ae-110">Some speakers and apps have their own volume controls, and you might have to check them all to make sure they're at the right levels.</span></span>
- <span data-ttu-id="4a9ae-111">Coba sambungkan menggunakan port USB yang berbeda.</span><span class="sxs-lookup"><span data-stu-id="4a9ae-111">Try connecting using a different USB port.</span></span>
- <span data-ttu-id="4a9ae-112">**Catatan:** Ingatlah bahwa speaker Anda mungkin tidak bekerja saat headphone dicolokkan.</span><span class="sxs-lookup"><span data-stu-id="4a9ae-112">**Note:** Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="4a9ae-113">**Periksa Device Manager**</span><span class="sxs-lookup"><span data-stu-id="4a9ae-113">**Check Device Manager**</span></span>

<span data-ttu-id="4a9ae-114">Untuk memastikan bahwa driver telah diperbarui:</span><span class="sxs-lookup"><span data-stu-id="4a9ae-114">To make sure the drivers are up to date:</span></span>

- <span data-ttu-id="4a9ae-115">Pilih **mulai**, ketik **Device Manager**, dan kemudian pilih **pengelola perangkat** dari daftar hasil.</span><span class="sxs-lookup"><span data-stu-id="4a9ae-115">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="4a9ae-116">Di bawah **kontrol suara, video, dan game**, pilih kartu suara, buka, pilih tab **driver** , dan pilih **Perbarui driver**.</span><span class="sxs-lookup"><span data-stu-id="4a9ae-116">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span> 

<span data-ttu-id="4a9ae-117">**Catatan:** Jika Windows tidak menemukan pengandar baru, Cari satu di situs web produsen perangkat dan ikuti petunjuk mereka.</span><span class="sxs-lookup"><span data-stu-id="4a9ae-117">**Note:** If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="4a9ae-118">**Instal ulang pengandar**</span><span class="sxs-lookup"><span data-stu-id="4a9ae-118">**Reinstall the driver**</span></span>

<span data-ttu-id="4a9ae-119">Jika Anda tidak dapat memperbarui melalui pengelola perangkat atau menemukan pengandar baru di situs web produsen, coba langkah-langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="4a9ae-119">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span> 

1. <span data-ttu-id="4a9ae-120">Pada pengelola perangkat, klik kanan (atau tekan dan tahan) pengandar audio, dan pilih **bongkar**.</span><span class="sxs-lookup"><span data-stu-id="4a9ae-120">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="4a9ae-121">Restart perangkat Anda dan Windows akan mencoba untuk menginstal ulang pengandar.</span><span class="sxs-lookup"><span data-stu-id="4a9ae-121">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="4a9ae-122">Jika menginstal ulang pengandar tidak bekerja, cobalah menggunakan pengandar audio generik yang datang dengan Windows.</span><span class="sxs-lookup"><span data-stu-id="4a9ae-122">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="4a9ae-123">Pada pengelola perangkat, klik kanan (atau tekan dan tahan) driver audio Anda > **Perbarui perangkat lunak** > **driver Jelajahi komputer saya untuk perangkat lunak** > pengandar**biarkan saya memilih dari daftar pengandar perangkat di komputer saya**, pilih **perangkat audio definisi tinggi**, pilih **berikutnya**, dan ikuti petunjuk untuk menginstalnya.</span><span class="sxs-lookup"><span data-stu-id="4a9ae-123">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>

<span data-ttu-id="4a9ae-124">**Mengatur perangkat default**</span><span class="sxs-lookup"><span data-stu-id="4a9ae-124">**Set the default device**</span></span>

<span data-ttu-id="4a9ae-125">Jika Anda tersambung ke perangkat audio menggunakan USB atau HDMI, Anda mungkin perlu menyetel perangkat tersebut sebagai default:</span><span class="sxs-lookup"><span data-stu-id="4a9ae-125">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span> 

1. <span data-ttu-id="4a9ae-126">Pilih **mulai**, ketik **suara**, dan kemudian pilih **suara** atau **mengubah suara sistem** dari daftar hasil.</span><span class="sxs-lookup"><span data-stu-id="4a9ae-126">Select **Start**, type **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2. <span data-ttu-id="4a9ae-127">Pada tab **pemutaran** , pilih perangkat, pilih **tetapkan default**, dan kemudian pilih **OK**.</span><span class="sxs-lookup"><span data-stu-id="4a9ae-127">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

