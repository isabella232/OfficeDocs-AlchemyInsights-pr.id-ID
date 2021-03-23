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
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036588"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="ed206-102">Mengosongkan ruang drive di Windows 10</span><span class="sxs-lookup"><span data-stu-id="ed206-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="ed206-103">Berikut adalah dua opsi untuk mengosongkan ruang drive di Windows:</span><span class="sxs-lookup"><span data-stu-id="ed206-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="ed206-104">Mengosongkan ruang drive di Windows 10.</span><span class="sxs-lookup"><span data-stu-id="ed206-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="ed206-105">Mengosongkan ruang untuk pembaruan Windows 10 dengan perangkat penyimpanan eksternal.</span><span class="sxs-lookup"><span data-stu-id="ed206-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="ed206-106">Jika Anda masih memiliki ruang disk yang rendah setelah menggunakan pembersihan disk, ada kemungkinan folder Temp Anda mengisi dengan file Application (. Appx) yang digunakan oleh Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="ed206-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="ed206-107">Untuk memperbaiki masalah ini, reset penyimpanan, kosongkan tembolok penyimpanan, lalu jalankan pemecah masalah pembaruan Windows.</span><span class="sxs-lookup"><span data-stu-id="ed206-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="ed206-108">Pastikan Microsoft Store ditutup sebelum Anda melanjutkan langkah-langkah ini.</span><span class="sxs-lookup"><span data-stu-id="ed206-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="ed206-109">**Langkah 1: mereset Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="ed206-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="ed206-110">**Catatan** Ini menghapus data aplikasi secara permanen pada perangkat, termasuk preferensi dan detail masuk Anda.</span><span class="sxs-lookup"><span data-stu-id="ed206-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="ed206-111">Pilih **mulai**  >  **pengaturan**  >  **aplikasi** aplikasi  >  **& fitur**.</span><span class="sxs-lookup"><span data-stu-id="ed206-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="ed206-112">Di daftar aplikasi, temukan dan pilih Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="ed206-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="ed206-113">Pilih **opsi tingkat lanjut**.</span><span class="sxs-lookup"><span data-stu-id="ed206-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="ed206-114">Gulir ke bawah dan pilih **reset**, lalu **konfirmasikan ulang**.</span><span class="sxs-lookup"><span data-stu-id="ed206-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="ed206-115">**Langkah 2: Kosongkan singgahan penyimpanan Microsoft**</span><span class="sxs-lookup"><span data-stu-id="ed206-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="ed206-116">Tekan tombol logo Windows + R untuk membuka kotak dialog Jalankan.</span><span class="sxs-lookup"><span data-stu-id="ed206-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="ed206-117">Ketik wsreset.exe dan pilih **OK**.</span><span class="sxs-lookup"><span data-stu-id="ed206-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="ed206-118">Jendela prompt perintah kosong terbuka.</span><span class="sxs-lookup"><span data-stu-id="ed206-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="ed206-119">Setelah sekitar 10 detik, jendela tertutup dan penyimpanan akan terbuka secara otomatis.</span><span class="sxs-lookup"><span data-stu-id="ed206-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="ed206-120">**Langkah 3: reset pembaruan Windows**</span><span class="sxs-lookup"><span data-stu-id="ed206-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="ed206-121">Pilih **mulai**  >  **pengaturan**  >  **pembaruan &**  >  **pemecahan masalah** keamanan.</span><span class="sxs-lookup"><span data-stu-id="ed206-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="ed206-122">Gulir ke bawah dan pilih **Windows Update** dari daftar, lalu pilih **Jalankan pemecah masalah**.</span><span class="sxs-lookup"><span data-stu-id="ed206-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="ed206-123">Hidupkan ulang komputer Anda dan periksa apakah Anda masih mengalami masalah tersebut.</span><span class="sxs-lookup"><span data-stu-id="ed206-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

