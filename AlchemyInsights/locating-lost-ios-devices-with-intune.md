---
title: Menemukan perangkat iOS yang hilang dengan Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439628"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="7c2fc-102">Menemukan perangkat iOS yang hilang dengan Intune</span><span class="sxs-lookup"><span data-stu-id="7c2fc-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="7c2fc-103">Mengaktifkan mode hilang pada perangkat iOS memungkinkan administrator untuk memiliki pesan dan nomor telepon kontak yang ditampilkan pada layar kunci.</span><span class="sxs-lookup"><span data-stu-id="7c2fc-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="7c2fc-104">Setelah mode hilang diaktifkan admin dapat menggunakan perangkat Cari tindakan untuk mengidentifikasi lokasi fisik perangkat.</span><span class="sxs-lookup"><span data-stu-id="7c2fc-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="7c2fc-105">Tindakan temukan perangkat di Intune bekerja dengan perangkat iOS untuk menampilkan lokasi perangkat tertentu pada peta.</span><span class="sxs-lookup"><span data-stu-id="7c2fc-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="7c2fc-106">Menggunakan tindakan ini memerlukan perangkat iOS untuk berada di:</span><span class="sxs-lookup"><span data-stu-id="7c2fc-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="7c2fc-107">Mode diawasi</span><span class="sxs-lookup"><span data-stu-id="7c2fc-107">Supervised mode</span></span>
- <span data-ttu-id="7c2fc-108">Mode hilang</span><span class="sxs-lookup"><span data-stu-id="7c2fc-108">Lost mode</span></span>

<span data-ttu-id="7c2fc-109">Untuk informasi lebih lanjut, lihat [mengaktifkan mode hilang pada perangkat iOS/ipados dengan Intune](https://docs.microsoft.com/intune/device-lost-mode) dan [menemukan perangkat iOS/ipados hilang atau dicuri dengan Intune](https://docs.microsoft.com/intune/device-locate).</span><span class="sxs-lookup"><span data-stu-id="7c2fc-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="7c2fc-110">**FAQ**</span><span class="sxs-lookup"><span data-stu-id="7c2fc-110">**FAQ**</span></span>

<span data-ttu-id="7c2fc-111">T: saya mengeluarkan tindakan jarak jauh untuk menghapus data perusahaan dari perangkat, dan sekarang terjebak dalam keadaan tertunda.</span><span class="sxs-lookup"><span data-stu-id="7c2fc-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="7c2fc-112">A: untuk tindakan jarak jauh untuk berhasil menyelesaikan, perangkat target harus online dan sehat.</span><span class="sxs-lookup"><span data-stu-id="7c2fc-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="7c2fc-113">Dalam situasi berikut, tindakan jarak jauh tetap dalam keadaan tertunda selama 30 hari, atau sampai perangkat mengakui perintah:</span><span class="sxs-lookup"><span data-stu-id="7c2fc-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="7c2fc-114">Bila perangkat tidak memiliki konektivitas</span><span class="sxs-lookup"><span data-stu-id="7c2fc-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="7c2fc-115">Ketika perangkat kehilangan status manajemen dengan Intune</span><span class="sxs-lookup"><span data-stu-id="7c2fc-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="7c2fc-116">Jika Anda merasa perangkat tidak lagi masuk, dan tidak dapat menghapus data perusahaan, pilih Hapus.</span><span class="sxs-lookup"><span data-stu-id="7c2fc-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="7c2fc-117">Menghapus menghapus rekaman perangkat sehingga tidak lagi muncul di Daftar perangkat Intune.</span><span class="sxs-lookup"><span data-stu-id="7c2fc-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="7c2fc-118">Jika perangkat aktif kembali, pengguna harus mendaftarkannya kembali.</span><span class="sxs-lookup"><span data-stu-id="7c2fc-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="7c2fc-119">T: Mengapa tindakan jarak jauh tertentu tidak tersedia bagi saya untuk digunakan?</span><span class="sxs-lookup"><span data-stu-id="7c2fc-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="7c2fc-120">A: tidak semua platform mendukung semua tindakan perangkat jarak jauh.</span><span class="sxs-lookup"><span data-stu-id="7c2fc-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="7c2fc-121">Tindakan jarak jauh berikut ini khusus platform, sehingga tersedia hanya untuk platform yang dicatat.</span><span class="sxs-lookup"><span data-stu-id="7c2fc-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="7c2fc-122">Kunci aktivasi bypass (hanya iOS)</span><span class="sxs-lookup"><span data-stu-id="7c2fc-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="7c2fc-123">Mulai segar (khusus Windows)</span><span class="sxs-lookup"><span data-stu-id="7c2fc-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="7c2fc-124">Mode hilang (khusus iOS)</span><span class="sxs-lookup"><span data-stu-id="7c2fc-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="7c2fc-125">Menemukan perangkat (khusus iOS)</span><span class="sxs-lookup"><span data-stu-id="7c2fc-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="7c2fc-126">Mulai ulang (khusus Windows)</span><span class="sxs-lookup"><span data-stu-id="7c2fc-126">Restart (Windows only)</span></span>

<span data-ttu-id="7c2fc-127">Untuk detail selengkapnya tentang setiap tindakan, lihat [tindakan perangkat yang tersedia](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="7c2fc-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>