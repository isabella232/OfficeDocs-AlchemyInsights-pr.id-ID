---
title: Bantuan terkait pengaturan tampilan cahaya malam
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404664"
---
# <a name="help-with-the-night-light-display-setting"></a><span data-ttu-id="f52de-102">Bantuan terkait pengaturan tampilan cahaya malam</span><span class="sxs-lookup"><span data-stu-id="f52de-102">Help with the night light display setting</span></span>

<span data-ttu-id="f52de-103">Untuk mempelajari selengkapnya tentang pengaturan tampilan waktu malam, [lihat Mengatur tampilan Anda untuk waktu malam di Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span><span class="sxs-lookup"><span data-stu-id="f52de-103">To learn more about night time display settings, see [Set your display for night time in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span></span>

<span data-ttu-id="f52de-104">Jika opsi cahaya malam berwarna abu-abu di Pengaturan, periksa driver tampilan Anda:</span><span class="sxs-lookup"><span data-stu-id="f52de-104">If the night light options are grayed out in Settings, check your display driver:</span></span> 

1. <span data-ttu-id="f52de-105">Klik kotak pencarian di taskbar Anda dan ketik **Manajer Perangkat**, lalu pilih **Manajer Perangkat** di hasil pencarian.</span><span class="sxs-lookup"><span data-stu-id="f52de-105">Click the search box on your taskbar and type **Device Manager**, and then select **Device Manager** in the search results.</span></span>
1. <span data-ttu-id="f52de-106">Perluas **Adaptor tampilan**.</span><span class="sxs-lookup"><span data-stu-id="f52de-106">Expand **Display adapters**.</span></span> 

<span data-ttu-id="f52de-107">Sayangnya, fitur cahaya malam tidak tersedia jika perangkat Anda menggunakan driver DisplayLink atau driver Tampilan Dasar.</span><span class="sxs-lookup"><span data-stu-id="f52de-107">Unfortunately, the night light feature is not available if your device uses a DisplayLink driver or a Basic Display driver.</span></span>

<span data-ttu-id="f52de-108">Fitur cahaya malam menggunakan teknologi grafik terbaru, sehingga Anda mungkin perlu memperbarui driver tampilan:</span><span class="sxs-lookup"><span data-stu-id="f52de-108">The night light feature makes use of recent graphics technology, so you might need to update your display driver:</span></span>  

- <span data-ttu-id="f52de-109">Periksa pembaruan dengan masuk ke Mulai  >  **Pengaturan**  >  **Pembaruan & Windows**  >  **Update** Periksa  >  **Pembaruan Windows.**</span><span class="sxs-lookup"><span data-stu-id="f52de-109">Check for updates by going to **Start** > **Settings** > **Update & Security** > **Windows Update** > **Check for Updates**.</span></span>  

<span data-ttu-id="f52de-110">ATAU</span><span class="sxs-lookup"><span data-stu-id="f52de-110">OR</span></span>

- <span data-ttu-id="f52de-111">Kunjungi situs web dukungan produsen perangkat keras Anda untuk mengunduh dan menginstal driver tampilan terbaru secara manual.</span><span class="sxs-lookup"><span data-stu-id="f52de-111">Visit your hardware manufacturer's support website to manually download and install the latest display drivers.</span></span>

## <a name="reset-night-light-in-the-registry"></a><span data-ttu-id="f52de-112">Mengatur ulang cahaya malam di registri</span><span class="sxs-lookup"><span data-stu-id="f52de-112">Reset night light in the registry</span></span>

<span data-ttu-id="f52de-113">Jika memperbarui driver tampilan tidak berfungsi, Anda mungkin perlu mengatur ulang lampu malam dalam registri.</span><span class="sxs-lookup"><span data-stu-id="f52de-113">If updating your display driver didn't work, you might need to reset night light in the registry.</span></span>  

<span data-ttu-id="f52de-114">**Perhatian:** Langkah pemecahan masalah ini disarankan hanya untuk pengguna tingkat lanjut.</span><span class="sxs-lookup"><span data-stu-id="f52de-114">**Caution:** This troubleshooting step is recommended only for advanced users.</span></span> <span data-ttu-id="f52de-115">Masalah serius dapat terjadi jika Anda salah mengubah registri.</span><span class="sxs-lookup"><span data-stu-id="f52de-115">Serious problems can occur if you modify the registry incorrectly.</span></span> <span data-ttu-id="f52de-116">Untuk perlindungan tambahan, buat cadangan registri sebelum mengubahnya agar Anda dapat memulihkannya jika terjadi masalah.</span><span class="sxs-lookup"><span data-stu-id="f52de-116">For added protection, back up the registry before you modify it so  you can restore it if problems occur.</span></span>

1. <span data-ttu-id="f52de-117">Dalam kotak pencarian, ketikkan **regedit**, lalu pilih **Editor Registri** dalam hasil pencarian.</span><span class="sxs-lookup"><span data-stu-id="f52de-117">In the search box, type **regedit**, and then select **Registry Editor** in the search results.</span></span>

1. <span data-ttu-id="f52de-118">Masuk ke kunci registri berikut:</span><span class="sxs-lookup"><span data-stu-id="f52de-118">Go to the following registry key:</span></span> 

    <span data-ttu-id="f52de-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span><span class="sxs-lookup"><span data-stu-id="f52de-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span></span>

1. <span data-ttu-id="f52de-120">Ekspor lalu hapus subkey berikut:$$windows.data.bluelightreduction.bluelightreductionstate</span><span class="sxs-lookup"><span data-stu-id="f52de-120">Export and then delete the following subkey:$$windows.data.bluelightreduction.bluelightreductionstate</span></span>

1. <span data-ttu-id="f52de-121">Ekspor lalu hapus subkey berikut:$$windows.data.bluelightreduction.settings</span><span class="sxs-lookup"><span data-stu-id="f52de-121">Export and then delete the following subkey:$$windows.data.bluelightreduction.settings</span></span>

1. <span data-ttu-id="f52de-122">Mulai ulang Windows dan pastikan apakah opsi cahaya malam tersedia.</span><span class="sxs-lookup"><span data-stu-id="f52de-122">Restart Windows and verify if the night light options are available.</span></span>


