---
title: Memecahkan masalah crash OneDrive
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
- "9003084"
- "5885"
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826202"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="4306f-102">Memecahkan masalah crash OneDrive</span><span class="sxs-lookup"><span data-stu-id="4306f-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="4306f-103">Jika OneDrive mengalami crash berulang kali, coba langkah-langkah pemecahan masalah berikut:</span><span class="sxs-lookup"><span data-stu-id="4306f-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="4306f-104">**Pastikan kunci registri tidak diatur:**</span><span class="sxs-lookup"><span data-stu-id="4306f-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="4306f-105">Menggunakan Editor Registri, navigasikan ke HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="4306f-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="4306f-106">Jika DisableFileSyncNGSC ada dan diatur ke 1, buka kunci dan ubah nilai ke 0.</span><span class="sxs-lookup"><span data-stu-id="4306f-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="4306f-107">Luncurkan OneDrive secara manual dengan membuka Mulai</span><span class="sxs-lookup"><span data-stu-id="4306f-107">Manually launch OneDrive by going to Start</span></span> ![Tekan tombol Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="4306f-109">, ketikkan OneDrive dalam kotak pencarian, lalu klik aplikasi desktop OneDrive.</span><span class="sxs-lookup"><span data-stu-id="4306f-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="4306f-110">**Mengatur ulang OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="4306f-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="4306f-111">Catatan:</span><span class="sxs-lookup"><span data-stu-id="4306f-111">Notes:</span></span>

- <span data-ttu-id="4306f-112">Mengatur ulang OneDrive akan memutuskan semua koneksi sinkronisasi yang ada (termasuk OneDrive pribadi, jika disiapkan).</span><span class="sxs-lookup"><span data-stu-id="4306f-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="4306f-113">Anda tidak akan kehilangan file atau data dengan mengatur ulang OneDrive di komputer.</span><span class="sxs-lookup"><span data-stu-id="4306f-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="4306f-114">**Untuk mengatur ulang OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="4306f-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="4306f-115">Buka dialog Jalankan dengan menekan tombol Windows dan R.</span><span class="sxs-lookup"><span data-stu-id="4306f-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="4306f-116">Ketik %localappdata%\Microsoft\OneDrive\onedrive.exe /reset, lalu tekan OK.</span><span class="sxs-lookup"><span data-stu-id="4306f-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="4306f-117">Jendela Perintah mungkin akan muncul sebentar.</span><span class="sxs-lookup"><span data-stu-id="4306f-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="4306f-118">Luncurkan OneDrive secara manual dengan membuka Mulai</span><span class="sxs-lookup"><span data-stu-id="4306f-118">Manually launch OneDrive by going to Start</span></span> ![Tekan tombol Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="4306f-120">, ketikkan OneDrive dalam kotak pencarian, lalu klik aplikasi desktop OneDrive.</span><span class="sxs-lookup"><span data-stu-id="4306f-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="4306f-121">Catatan:</span><span class="sxs-lookup"><span data-stu-id="4306f-121">Notes:</span></span>

- <span data-ttu-id="4306f-122">Jika memilih untuk menyinkronkan beberapa folder saja sebelum mengatur ulang, Anda perlu melakukannya lagi setelah sinkronisasi selesai.</span><span class="sxs-lookup"><span data-stu-id="4306f-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="4306f-123">Baca [Memilih folder OneDrive yang akan disinkronkan ke komputer untuk](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)informasi   selengkapnya.</span><span class="sxs-lookup"><span data-stu-id="4306f-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="4306f-124">Anda harus menyelesaikan ini untuk OneDrive pribadi dan OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="4306f-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>