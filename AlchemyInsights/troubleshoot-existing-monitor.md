---
title: Memecahkan masalah monitor yang sudah ada
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
- "3454"
- "9001450"
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824582"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="663ae-102">Memecahkan masalah monitor yang sudah ada</span><span class="sxs-lookup"><span data-stu-id="663ae-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="663ae-103">Cobalah solusi ini untuk memecahkan masalah monitor.</span><span class="sxs-lookup"><span data-stu-id="663ae-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="663ae-104">**Refresh tampilan monitor Anda:**</span><span class="sxs-lookup"><span data-stu-id="663ae-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="663ae-105">Tekan tombol berikut secara bersamaan: Tombol Windows + Ctrl + Shift + B. Ini akan merefresh komunikasi dengan driver grafik Anda.</span><span class="sxs-lookup"><span data-stu-id="663ae-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="663ae-106">Monitor Anda akan berkedip sementara waktu dan kembali setelah beberapa detik.</span><span class="sxs-lookup"><span data-stu-id="663ae-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="663ae-107">**Memecahkan masalah perangkat keras monitor:**</span><span class="sxs-lookup"><span data-stu-id="663ae-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="663ae-108">Cabut kabel yang menghubungkan PC Anda ke monitor Anda, dan sambungkan kembali.</span><span class="sxs-lookup"><span data-stu-id="663ae-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="663ae-109">Putuskan sambungan perangkat non-esensial dari PC Anda (seperti adaptor atau dok).</span><span class="sxs-lookup"><span data-stu-id="663ae-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="663ae-110">**Jika baru saja menginstal pembaruan di PC, Anda dapat mengembalikan driver tampilan:**</span><span class="sxs-lookup"><span data-stu-id="663ae-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="663ae-111">Pilih **Mulai**, ketik **manajer perangkat**, dan pilih Manajer **Perangkat** dari hasil.</span><span class="sxs-lookup"><span data-stu-id="663ae-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="663ae-112">Perluas **bagian Adaptor tampilan,** klik kanan adaptor tampilan Anda, lalu pilih **Properti**.</span><span class="sxs-lookup"><span data-stu-id="663ae-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="663ae-113">Navigasikan ke tab **Driver,** lalu **pilih Kembalikan Driver.**</span><span class="sxs-lookup"><span data-stu-id="663ae-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="663ae-114">Catatan: Jika opsi ini tidak tersedia atau berwarna abu-abu, pilih **Tidak** dari opsi di bawah ini untuk melanjutkan ke langkah berikutnya.</span><span class="sxs-lookup"><span data-stu-id="663ae-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="663ae-115">Anda mungkin perlu memulai ulang PC sebelum perubahan ini diterapkan.</span><span class="sxs-lookup"><span data-stu-id="663ae-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="663ae-116">**Hapus instalan dan instal ulang driver tampilan Anda:**</span><span class="sxs-lookup"><span data-stu-id="663ae-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="663ae-117">Pilih **Mulai**, ketik **manajer perangkat**, dan pilih Manajer **Perangkat** dari hasil.</span><span class="sxs-lookup"><span data-stu-id="663ae-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="663ae-118">Perluas **bagian Adaptor tampilan,** klik kanan adaptor tampilan Anda, lalu pilih Hapus **instalan perangkat**.</span><span class="sxs-lookup"><span data-stu-id="663ae-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="663ae-119">Pilih kotak di samping Hapus **perangkat lunak driver untuk perangkat ini, lalu** pilih Hapus **instalan**.</span><span class="sxs-lookup"><span data-stu-id="663ae-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="663ae-120">Catatan: Anda mungkin diminta untuk memulai ulang komputer pada tahap ini.</span><span class="sxs-lookup"><span data-stu-id="663ae-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="663ae-121">Pastikan untuk menuliskan instruksi selanjutnya sebelum memulai ulang.</span><span class="sxs-lookup"><span data-stu-id="663ae-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="663ae-122">Buka Manajer Perangkat lagi.</span><span class="sxs-lookup"><span data-stu-id="663ae-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="663ae-123">Perluas **bagian Adaptor tampilan,** klik kanan adaptor tampilan Anda, lalu pilih **Perbarui Driver**.</span><span class="sxs-lookup"><span data-stu-id="663ae-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="663ae-124">Pilih **Cari perangkat lunak driver pembaruan secara otomatis** dan ikuti instruksi penginstalan.</span><span class="sxs-lookup"><span data-stu-id="663ae-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>