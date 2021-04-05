---
title: Mengosongkan ruang drive di Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505359"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="4e2e7-102">Mengosongkan ruang drive di Windows 10</span><span class="sxs-lookup"><span data-stu-id="4e2e7-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="4e2e7-103">Ada dua opsi untuk mengosongkan ruang drive di Windows:</span><span class="sxs-lookup"><span data-stu-id="4e2e7-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="4e2e7-104">Mengosongkan ruang drive di Windows 10.</span><span class="sxs-lookup"><span data-stu-id="4e2e7-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="4e2e7-105">Kosongkan ruang untuk pembaruan Windows 10 dengan perangkat penyimpanan eksternal.</span><span class="sxs-lookup"><span data-stu-id="4e2e7-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="4e2e7-106">Jika ruang disk masih rendah setelah menggunakan Pembersihan Disk, kemungkinan folder Temp Anda dengan cepat terisi file aplikasi (.appx) yang digunakan oleh Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="4e2e7-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="4e2e7-107">Untuk memperbaiki masalah ini, atur ulang Store, bersihkan cache Store, lalu jalankan pemecah masalah Windows Update.</span><span class="sxs-lookup"><span data-stu-id="4e2e7-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="4e2e7-108">Pastikan Microsoft Store ditutup sebelum Anda melanjutkan ke langkah-langkah berikut.</span><span class="sxs-lookup"><span data-stu-id="4e2e7-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="4e2e7-109">**Langkah 1: Atur ulang Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="4e2e7-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="4e2e7-110">**Catatan** Tindakan ini akan menghapus permanen data aplikasi di perangkat, termasuk preferensi Anda dan detail masuk.</span><span class="sxs-lookup"><span data-stu-id="4e2e7-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="4e2e7-111">Pilih **Mulai** > **Pengaturan** > **Aplikasi** > **Aplikasi & fitur**.</span><span class="sxs-lookup"><span data-stu-id="4e2e7-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="4e2e7-112">Di daftar aplikasi, temukan dan pilih Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="4e2e7-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="4e2e7-113">Pilih **Opsi lanjutan**.</span><span class="sxs-lookup"><span data-stu-id="4e2e7-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="4e2e7-114">Gulir ke bawah dan pilih **Atur Ulang**, lalu **Konfirmasi Atur Ulang**.</span><span class="sxs-lookup"><span data-stu-id="4e2e7-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="4e2e7-115">**Langkah 2: Bersihkan cache Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="4e2e7-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="4e2e7-116">Tekan Tombol Logo Windows + R untuk membuka Jalankan kotak dialog.</span><span class="sxs-lookup"><span data-stu-id="4e2e7-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="4e2e7-117">Ketik wsreset.exe lalu pilih **OK**.</span><span class="sxs-lookup"><span data-stu-id="4e2e7-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="4e2e7-118">Jendela Perintah kosong akan terbuka.</span><span class="sxs-lookup"><span data-stu-id="4e2e7-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="4e2e7-119">Setelah sekitar 10 detik, jendela tersebut akan tertutup dan Store akan terbuka secara otomatis.</span><span class="sxs-lookup"><span data-stu-id="4e2e7-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="4e2e7-120">**Langkah 3: Atur Ulang Windows Update**</span><span class="sxs-lookup"><span data-stu-id="4e2e7-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="4e2e7-121">Pilih **Mulai** > **Pengaturan** > **Pembaruan & Keamanan** > **Pemecahan Masalah**.</span><span class="sxs-lookup"><span data-stu-id="4e2e7-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="4e2e7-122">Gulir ke bawah dan pilih **Windows Update** dari daftar, lalu pilih **Jalankan pemecah masalah**.</span><span class="sxs-lookup"><span data-stu-id="4e2e7-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="4e2e7-123">Boot ulang komputer, lalu periksa apakah Anda masih mengalami masalah tersebut.</span><span class="sxs-lookup"><span data-stu-id="4e2e7-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

