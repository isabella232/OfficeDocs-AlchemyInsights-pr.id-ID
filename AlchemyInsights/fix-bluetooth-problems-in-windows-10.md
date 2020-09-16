---
title: Memperbaiki masalah Bluetooth di Windows 10
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
- "9001475"
- "3506"
ms.openlocfilehash: 7e7a397a1f6777972a81bcbb6bffa1c98d8370a4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730162"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="5b994-102">Memperbaiki masalah Bluetooth di Windows 10</span><span class="sxs-lookup"><span data-stu-id="5b994-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="5b994-103">Jika ikon Bluetooth hilang atau tidak dapat diaktifkan atau dinonaktifkan, Anda mungkin ingin menjalankan pemecah masalah Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="5b994-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="5b994-104">[Buka pengaturan pemecahan masalah](ms-settings:troubleshoot), klik **Bluetooth** di bawah **Temukan dan Perbaiki masalah lainnya**, klik **Jalankan pemecah**masalah.</span><span class="sxs-lookup"><span data-stu-id="5b994-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="5b994-105">Jika Anda tidak melihat ikon Bluetooth, tapi Bluetooth muncul di manajer perangkat:</span><span class="sxs-lookup"><span data-stu-id="5b994-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="5b994-106">Di manajer perangkat, klik **Bluetooth**.</span><span class="sxs-lookup"><span data-stu-id="5b994-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="5b994-107">Tekan dan tahan (atau klik kanan) nama adaptor Bluetooth dan klik **hapus instalan perangkat**.</span><span class="sxs-lookup"><span data-stu-id="5b994-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="5b994-108">Matikan perangkat Windows Anda, tunggu beberapa detik, lalu nyalakan kembali.</span><span class="sxs-lookup"><span data-stu-id="5b994-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="5b994-109">Windows akan mencoba menginstal ulang driver.</span><span class="sxs-lookup"><span data-stu-id="5b994-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="5b994-110">Jika Anda baru saja menginstal pembaruan Windows 10 atau memutakhirkan ke Windows 10, Anda mungkin ingin memeriksa pembaruan driver:</span><span class="sxs-lookup"><span data-stu-id="5b994-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="5b994-111">Di manajer perangkat, klik **Bluetooth**, lalu klik nama adaptor Bluetooth (yang mungkin menyertakan kata "radio").</span><span class="sxs-lookup"><span data-stu-id="5b994-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="5b994-112">Tekan dan tahan (atau klik kanan) adapter Bluetooth, lalu klik **Perbarui**  >  **pencarian driver secara otomatis untuk perangkat lunak driver yang diperbarui**.</span><span class="sxs-lookup"><span data-stu-id="5b994-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="5b994-113">Ikuti langkah-langkahnya, lalu klik **tutup**.</span><span class="sxs-lookup"><span data-stu-id="5b994-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="5b994-114">Jika Windows tidak dapat menemukan driver Bluetooth baru, kunjungi situs web pabrikan PC dan Unduh driver Bluetooth terbaru dari sana.</span><span class="sxs-lookup"><span data-stu-id="5b994-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="5b994-115">Setelah Anda mengunduhnya, klik **Perbarui pengandar**  >  **Telusuri komputer saya untuk menelusuri perangkat lunak pengandar**  >  **Browse** untuk lokasi tempat file pengandar disimpan > **OK**  >  **berikutnya**, dan ikuti langkah-langkah untuk menginstal.</span><span class="sxs-lookup"><span data-stu-id="5b994-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="5b994-116">Setelah menginstal driver yang diperbarui, mulai ulang komputer, lalu Periksa apakah masalah koneksi telah diperbaiki.</span><span class="sxs-lookup"><span data-stu-id="5b994-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="5b994-117">Untuk detail selengkapnya tentang cara memecahkan masalah Bluetooth, silakan lihat artikel lengkapnya, [Perbaiki masalah Bluetooth di Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span><span class="sxs-lookup"><span data-stu-id="5b994-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
