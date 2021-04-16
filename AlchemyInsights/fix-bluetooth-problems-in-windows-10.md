---
title: Memperbaiki masalah Bluetooth di Windows 10
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
- "9001475"
- "3506"
ms.openlocfilehash: f20bf4a642e019c7901e988a027e0220f0f1b07b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812935"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="c164c-102">Memperbaiki masalah Bluetooth di Windows 10</span><span class="sxs-lookup"><span data-stu-id="c164c-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="c164c-103">Jika ikon Bluetooth hilang atau Bluetooth tidak dapat diaktifkan atau dinonaktifkan, Anda mungkin ingin menjalankan pemecah masalah Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="c164c-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="c164c-104">[Buka pengaturan Pemecahan masalah,](ms-settings:troubleshoot)klik **Bluetooth di** **bawah Temukan dan perbaiki masalah** lain, klik Jalankan **pemecah masalah**.</span><span class="sxs-lookup"><span data-stu-id="c164c-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="c164c-105">Jika Anda tidak melihat ikon Bluetooth, tetapi Bluetooth muncul di Manajer Perangkat:</span><span class="sxs-lookup"><span data-stu-id="c164c-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="c164c-106">Di Manajer Perangkat, klik **Bluetooth.**</span><span class="sxs-lookup"><span data-stu-id="c164c-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="c164c-107">Tekan dan tahan (atau klik kanan) nama adaptor Bluetooth dan klik Hapus **instalan perangkat**.</span><span class="sxs-lookup"><span data-stu-id="c164c-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="c164c-108">Matikan perangkat Windows Anda, tunggu beberapa detik, lalu aktifkan kembali.</span><span class="sxs-lookup"><span data-stu-id="c164c-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="c164c-109">Windows akan mencoba menginstal ulang driver.</span><span class="sxs-lookup"><span data-stu-id="c164c-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="c164c-110">Jika Anda baru saja menginstal pembaruan Windows 10 atau meningkatkannya ke Windows 10, Anda mungkin perlu memeriksa pembaruan driver:</span><span class="sxs-lookup"><span data-stu-id="c164c-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="c164c-111">Di Manajer Perangkat, **klik Bluetooth**, lalu klik nama adaptor Bluetooth (yang mungkin menyertakan kata "radio").</span><span class="sxs-lookup"><span data-stu-id="c164c-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="c164c-112">Tekan dan tahan (atau klik kanan) adaptor Bluetooth, lalu klik Perbarui **driver Cari perangkat** lunak driver yang diperbarui secara  >  **otomatis.**</span><span class="sxs-lookup"><span data-stu-id="c164c-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="c164c-113">Ikuti langkah-langkah, lalu klik **Tutup.**</span><span class="sxs-lookup"><span data-stu-id="c164c-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="c164c-114">Jika Windows tidak dapat menemukan driver Bluetooth baru, kunjungi situs web produsen PC dan unduh driver Bluetooth terbaru dari sana.</span><span class="sxs-lookup"><span data-stu-id="c164c-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="c164c-115">Setelah Anda mengunduhnya, klik Perbarui **driver** Telusuri komputer saya untuk perangkat lunak driver Telusuri lokasi tempat file  >    >   driver disimpan > **OK**  >  Berikutnya, dan ikuti langkah-langkah untuk menginstal.</span><span class="sxs-lookup"><span data-stu-id="c164c-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="c164c-116">Setelah menginstal driver yang diperbarui, hidupkan ulang komputer, lalu periksa apakah masalah tersebut memperbaiki masalah koneksi.</span><span class="sxs-lookup"><span data-stu-id="c164c-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="c164c-117">Untuk detail selengkapnya tentang cara memecahkan masalah Bluetooth, lihat artikel lengkap, [Memperbaiki masalah Bluetooth di Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span><span class="sxs-lookup"><span data-stu-id="c164c-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
