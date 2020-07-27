---
title: Bypass aktivasi kunci pada perangkat iOS diawasi dengan Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423731"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a><span data-ttu-id="ad6d5-102">Bypass aktivasi kunci pada perangkat iOS diawasi dengan Intune</span><span class="sxs-lookup"><span data-stu-id="ad6d5-102">Bypass activation lock on supervised iOS devices with Intune</span></span>

<span data-ttu-id="ad6d5-103">Kemampuan untuk melewati kunci aktivasi pada perangkat iOS membuatnya lebih mudah untuk pulih dari skenario di mana pengguna mengaktifkan kunci aktivasi pada perangkat korporat, dan kemudian meninggalkan perusahaan.</span><span class="sxs-lookup"><span data-stu-id="ad6d5-103">The ability to bypass the activation lock on iOS devices makes it easier to recover from the scenario where a user enables activation lock on a corporate device, and then leaves the company.</span></span>

<span data-ttu-id="ad6d5-104">Prasyarat untuk melewati kunci aktivasi meliputi:</span><span class="sxs-lookup"><span data-stu-id="ad6d5-104">Pre-requisites to bypassing an activation lock include:</span></span>

- <span data-ttu-id="ad6d5-105">Perangkat adalah "diawasi."</span><span class="sxs-lookup"><span data-stu-id="ad6d5-105">A device is that is "supervised."</span></span>
- <span data-ttu-id="ad6d5-106">Kunci aktivasi berhasil diaktifkan menggunakan kebijakan pembatasan iOS perangkat di Intune.</span><span class="sxs-lookup"><span data-stu-id="ad6d5-106">The activation lock is successfully enabled using iOS Device restriction policy in Intune.</span></span>

<span data-ttu-id="ad6d5-107">Selain itu, ketika melewati kunci aktivasi, Anda harus:</span><span class="sxs-lookup"><span data-stu-id="ad6d5-107">In addition, when bypassing an activation lock, you should:</span></span>

- <span data-ttu-id="ad6d5-108">Fisik memiliki perangkat yang dihapus.</span><span class="sxs-lookup"><span data-stu-id="ad6d5-108">Physically possess the device being wiped.</span></span>
- <span data-ttu-id="ad6d5-109">Salin kode sebelum Anda mengeluarkan penghapusan.</span><span class="sxs-lookup"><span data-stu-id="ad6d5-109">Copy the code before you issue the wipe.</span></span>

<span data-ttu-id="ad6d5-110">**Catatan:** Kode wipe tidak case sensitive, sehingga karakter "-" tidak diperlukan.</span><span class="sxs-lookup"><span data-stu-id="ad6d5-110">**Note:** The wipe code is not case sensitive, so the "-" characters are not required.</span></span>

<span data-ttu-id="ad6d5-111">Untuk detailnya, lihat [bypass kunci aktivasi pada perangkat iOS yang diawasi dengan Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span><span class="sxs-lookup"><span data-stu-id="ad6d5-111">For details, see [Bypass Activation Lock on Supervised iOS devices with Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span></span>

<span data-ttu-id="ad6d5-112">**FAQ**</span><span class="sxs-lookup"><span data-stu-id="ad6d5-112">**FAQ**</span></span>

<span data-ttu-id="ad6d5-113">Q: **saya mengeluarkan tindakan jauh untuk menghapus data perusahaan dari perangkat, dan sekarang terjebak dalam keadaan tertunda.**</span><span class="sxs-lookup"><span data-stu-id="ad6d5-113">Q: **I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.**</span></span>

<span data-ttu-id="ad6d5-114">A: untuk tindakan jarak jauh untuk berhasil menyelesaikan, perangkat target harus online dan sehat.</span><span class="sxs-lookup"><span data-stu-id="ad6d5-114">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="ad6d5-115">Dalam situasi berikut, tindakan jarak jauh tetap dalam keadaan tertunda selama 30 hari, atau sampai perangkat mengakui perintah saat perangkat:</span><span class="sxs-lookup"><span data-stu-id="ad6d5-115">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command when the device:</span></span>

- <span data-ttu-id="ad6d5-116">Tidak memiliki konektivitas.</span><span class="sxs-lookup"><span data-stu-id="ad6d5-116">Does not have connectivity.</span></span>
- <span data-ttu-id="ad6d5-117">Kehilangan status manajemennya dengan Intune.</span><span class="sxs-lookup"><span data-stu-id="ad6d5-117">Loses its management status with Intune.</span></span>

<span data-ttu-id="ad6d5-118">Jika Anda merasa perangkat tidak lagi dapat memeriksa, dan tidak akan menghapus data perusahaan, pilih Hapus.</span><span class="sxs-lookup"><span data-stu-id="ad6d5-118">If you think a device is no longer checking in, and that it won’t remove company data, select Delete.</span></span> <span data-ttu-id="ad6d5-119">Menghapus menghapus rekaman perangkat sehingga tidak lagi muncul di Daftar perangkat Intune.</span><span class="sxs-lookup"><span data-stu-id="ad6d5-119">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="ad6d5-120">Agar perangkat aktif kembali, pengguna harus mendaftarkan ulang perangkat.</span><span class="sxs-lookup"><span data-stu-id="ad6d5-120">For the device to become active again, its user must re-enroll the device.</span></span>

<span data-ttu-id="ad6d5-121">T: **mengapa tindakan jarak jauh tertentu tidak tersedia bagi saya untuk digunakan?**</span><span class="sxs-lookup"><span data-stu-id="ad6d5-121">Q: **Why are certain remote actions not available for me to use?**</span></span>

<span data-ttu-id="ad6d5-122">A: tidak semua platform mendukung semua tindakan perangkat jarak jauh.</span><span class="sxs-lookup"><span data-stu-id="ad6d5-122">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="ad6d5-123">Tindakan jarak jauh berikut ini khusus platform.</span><span class="sxs-lookup"><span data-stu-id="ad6d5-123">The following remote actions are platform-specific.</span></span>

- <span data-ttu-id="ad6d5-124">Kunci aktivasi bypass (hanya iOS)</span><span class="sxs-lookup"><span data-stu-id="ad6d5-124">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="ad6d5-125">Mulai segar (khusus Windows)</span><span class="sxs-lookup"><span data-stu-id="ad6d5-125">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="ad6d5-126">Mode hilang (khusus iOS)</span><span class="sxs-lookup"><span data-stu-id="ad6d5-126">Lost mode (iOS only)</span></span>
- <span data-ttu-id="ad6d5-127">Menemukan perangkat (khusus iOS)</span><span class="sxs-lookup"><span data-stu-id="ad6d5-127">Locate device (iOS only)</span></span>
- <span data-ttu-id="ad6d5-128">Mulai ulang (khusus Windows)</span><span class="sxs-lookup"><span data-stu-id="ad6d5-128">Restart (Windows only)</span></span>

<span data-ttu-id="ad6d5-129">Untuk detail selengkapnya tentang setiap tindakan, lihat [tindakan perangkat yang tersedia](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="ad6d5-129">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>