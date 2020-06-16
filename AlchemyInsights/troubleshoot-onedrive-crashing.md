---
title: Memecahkan masalah OneDrive lumpuh
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/15/2020
ms.locfileid: "44749172"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="2400e-102">Memecahkan masalah OneDrive lumpuh</span><span class="sxs-lookup"><span data-stu-id="2400e-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="2400e-103">Jika OneDrive berulang kali lumpuh, cobalah langkah pemecahan masalah berikut:</span><span class="sxs-lookup"><span data-stu-id="2400e-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="2400e-104">**Pastikan kunci registri tidak ditetapkan:**</span><span class="sxs-lookup"><span data-stu-id="2400e-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="2400e-105">Menggunakan Penyunting registri, navigasikan ke HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="2400e-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="2400e-106">Jika DisableFileSyncNGSC ada dan disetel ke 1, buka kunci dan mengubah nilai ke 0.</span><span class="sxs-lookup"><span data-stu-id="2400e-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="2400e-107">Secara manual meluncurkan OneDrive dengan pergi ke Start</span><span class="sxs-lookup"><span data-stu-id="2400e-107">Manually launch OneDrive by going to Start</span></span> ![Tekan tombol Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="2400e-109">, ketik OneDrive di kotak pencarian, dan kemudian klik pada aplikasi OneDrive desktop.</span><span class="sxs-lookup"><span data-stu-id="2400e-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="2400e-110">**Setel ulang OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="2400e-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="2400e-111">Catatan:</span><span class="sxs-lookup"><span data-stu-id="2400e-111">Notes:</span></span>

- <span data-ttu-id="2400e-112">Mengatur ulang OneDrive terputus semua koneksi sinkronisasi yang ada (termasuk OneDrive pribadi Anda jika disiapkan).</span><span class="sxs-lookup"><span data-stu-id="2400e-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="2400e-113">Anda tidak akan kehilangan file atau data dengan menyetel ulang OneDrive pada komputer Anda.</span><span class="sxs-lookup"><span data-stu-id="2400e-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="2400e-114">**Untuk me-reset OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="2400e-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="2400e-115">Buka dialog jalankan dengan menekan tombol Windows dan R.</span><span class="sxs-lookup"><span data-stu-id="2400e-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="2400e-116">Ketik% localappdata% \Microsoft\OneDrive\onedrive.exe/reset dan tekan OK.</span><span class="sxs-lookup"><span data-stu-id="2400e-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="2400e-117">Jendela perintah akan muncul sebentar.</span><span class="sxs-lookup"><span data-stu-id="2400e-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="2400e-118">Secara manual meluncurkan OneDrive dengan pergi ke Start</span><span class="sxs-lookup"><span data-stu-id="2400e-118">Manually launch OneDrive by going to Start</span></span> ![Tekan tombol Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="2400e-120">, ketik OneDrive di kotak pencarian, dan kemudian klik pada aplikasi OneDrive desktop.</span><span class="sxs-lookup"><span data-stu-id="2400e-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="2400e-121">Catatan:</span><span class="sxs-lookup"><span data-stu-id="2400e-121">Notes:</span></span>

- <span data-ttu-id="2400e-122">Jika Anda telah memilih untuk melakukan sinkronisasi hanya beberapa folder sebelum reset, Anda akan perlu untuk melakukan itu lagi setelah sinkronisasi selesai.</span><span class="sxs-lookup"><span data-stu-id="2400e-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="2400e-123">Baca [memilih folder OneDrive yang akan disinkronkan ke komputer Anda](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   untuk informasi lebih lanjut.</span><span class="sxs-lookup"><span data-stu-id="2400e-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="2400e-124">Anda akan perlu untuk melengkapi ini untuk OneDrive pribadi Anda dan OneDrive untuk bisnis.</span><span class="sxs-lookup"><span data-stu-id="2400e-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>