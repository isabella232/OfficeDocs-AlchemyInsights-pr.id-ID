---
title: Pemecahan masalah monitor yang sudah ada
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
- "3454"
- "9001450"
ms.openlocfilehash: 2dc9a24c1d0d808e26733738cedbc32d513926a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690714"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="d88fb-102">Memecahkan masalah monitor yang sudah ada</span><span class="sxs-lookup"><span data-stu-id="d88fb-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="d88fb-103">Cobalah solusi ini untuk memecahkan masalah monitor.</span><span class="sxs-lookup"><span data-stu-id="d88fb-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="d88fb-104">**Refresh tampilan monitor Anda:**</span><span class="sxs-lookup"><span data-stu-id="d88fb-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="d88fb-105">Tekan tombol berikut ini pada saat yang sama: tombol Windows + Ctrl + Shift + B. Ini akan melakukan refresh komunikasi dengan driver grafis Anda.</span><span class="sxs-lookup"><span data-stu-id="d88fb-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="d88fb-106">Monitor akan berkedip sebentar dan kembali setelah beberapa detik.</span><span class="sxs-lookup"><span data-stu-id="d88fb-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="d88fb-107">**Memecahkan masalah perangkat keras monitor:**</span><span class="sxs-lookup"><span data-stu-id="d88fb-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="d88fb-108">Cabut kabel yang menyambungkan PC ke monitor, lalu sambungkan kembali.</span><span class="sxs-lookup"><span data-stu-id="d88fb-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="d88fb-109">Putuskan koneksi perangkat apa pun yang tidak penting dari PC Anda (seperti adapter atau Dock).</span><span class="sxs-lookup"><span data-stu-id="d88fb-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="d88fb-110">**Jika Anda baru saja menginstal pembaruan di PC, Anda bisa memutar kembali driver tampilan Anda:**</span><span class="sxs-lookup"><span data-stu-id="d88fb-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="d88fb-111">Pilih **mulai**, ketikkan **manajer perangkat**, lalu pilih **pengelola perangkat** dari hasil.</span><span class="sxs-lookup"><span data-stu-id="d88fb-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="d88fb-112">Perluas bagian **Adapter tampilan** , klik kanan Adapter tampilan Anda, ands pilih **properti**.</span><span class="sxs-lookup"><span data-stu-id="d88fb-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="d88fb-113">Navigasikan ke tab **pengandar** dan pilih **putar kembali pengandar**.</span><span class="sxs-lookup"><span data-stu-id="d88fb-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="d88fb-114">Catatan: jika ini tidak tersedia atau berwarna abu-abu, pilih **tidak** dari opsi di bawah ini untuk berpindah ke langkah berikutnya.</span><span class="sxs-lookup"><span data-stu-id="d88fb-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="d88fb-115">Anda mungkin perlu memulai ulang PC sebelum perubahan ini diterapkan.</span><span class="sxs-lookup"><span data-stu-id="d88fb-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="d88fb-116">**Hapus instalan dan instal ulang driver tampilan Anda:**</span><span class="sxs-lookup"><span data-stu-id="d88fb-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="d88fb-117">Pilih **mulai**, ketikkan **manajer perangkat**, lalu pilih **pengelola perangkat** dari hasil.</span><span class="sxs-lookup"><span data-stu-id="d88fb-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="d88fb-118">Perluas bagian **Adapter tampilan** , klik kanan adaptor tampilan Anda, ands pilih **Hapus perangkat**.</span><span class="sxs-lookup"><span data-stu-id="d88fb-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="d88fb-119">Pilih kotak di samping **Hapus perangkat lunak pengandar untuk perangkat ini,** lalu pilih **hapus instalan**.</span><span class="sxs-lookup"><span data-stu-id="d88fb-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="d88fb-120">Catatan: Anda mungkin diminta untuk memulai ulang komputer Anda pada tahap ini.</span><span class="sxs-lookup"><span data-stu-id="d88fb-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="d88fb-121">Pastikan untuk menuliskan instruksi yang tersisa sebelum Anda memulai ulang.</span><span class="sxs-lookup"><span data-stu-id="d88fb-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="d88fb-122">Buka Manajer perangkat lagi.</span><span class="sxs-lookup"><span data-stu-id="d88fb-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="d88fb-123">Perluas bagian **Adapter tampilan** , klik kanan Adapter tampilan Anda, lalu pilih **Perbarui driver**.</span><span class="sxs-lookup"><span data-stu-id="d88fb-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="d88fb-124">Pilih **Cari secara otomatis untuk memperbarui perangkat lunak pengandar** dan ikuti instruksi instalasi.</span><span class="sxs-lookup"><span data-stu-id="d88fb-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>