---
title: Memecahkan masalah OneDrive crash
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665001"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="646aa-102">Memecahkan masalah OneDrive crash</span><span class="sxs-lookup"><span data-stu-id="646aa-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="646aa-103">Jika OneDrive berulang kali mengalami crash, coba langkah pemecahan masalah ini:</span><span class="sxs-lookup"><span data-stu-id="646aa-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="646aa-104">**Pastikan kunci registri tidak diatur:**</span><span class="sxs-lookup"><span data-stu-id="646aa-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="646aa-105">Menggunakan editor registri, navigasikan ke HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="646aa-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="646aa-106">Jika DisableFileSyncNGSC ada dan disetel ke 1, buka kunci dan Ubah nilainya ke 0.</span><span class="sxs-lookup"><span data-stu-id="646aa-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="646aa-107">Luncurkan OneDrive secara manual dengan masuk ke mulai</span><span class="sxs-lookup"><span data-stu-id="646aa-107">Manually launch OneDrive by going to Start</span></span> ![Tekan tombol Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="646aa-109">, ketikkan OneDrive dalam kotak pencarian, lalu klik aplikasi desktop OneDrive.</span><span class="sxs-lookup"><span data-stu-id="646aa-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="646aa-110">**Atur ulang OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="646aa-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="646aa-111">Catatan</span><span class="sxs-lookup"><span data-stu-id="646aa-111">Notes:</span></span>

- <span data-ttu-id="646aa-112">Mereset OneDrive memutus semua koneksi sinkronisasi yang ada (termasuk OneDrive pribadi jika disetel).</span><span class="sxs-lookup"><span data-stu-id="646aa-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="646aa-113">Anda tidak akan kehilangan file atau data dengan mengatur ulang OneDrive di komputer Anda.</span><span class="sxs-lookup"><span data-stu-id="646aa-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="646aa-114">**Untuk mengatur ulang OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="646aa-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="646aa-115">Buka dialog jalankan dengan menekan tombol Windows dan R.</span><span class="sxs-lookup"><span data-stu-id="646aa-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="646aa-116">Ketikkan% localappdata% \Microsoft\OneDrive\onedrive.exe/reset dan tekan OK.</span><span class="sxs-lookup"><span data-stu-id="646aa-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="646aa-117">Jendela perintah mungkin muncul sebentar.</span><span class="sxs-lookup"><span data-stu-id="646aa-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="646aa-118">Luncurkan OneDrive secara manual dengan masuk ke mulai</span><span class="sxs-lookup"><span data-stu-id="646aa-118">Manually launch OneDrive by going to Start</span></span> ![Tekan tombol Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="646aa-120">, ketikkan OneDrive dalam kotak pencarian, lalu klik aplikasi desktop OneDrive.</span><span class="sxs-lookup"><span data-stu-id="646aa-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="646aa-121">Catatan</span><span class="sxs-lookup"><span data-stu-id="646aa-121">Notes:</span></span>

- <span data-ttu-id="646aa-122">Jika Anda telah memilih untuk menyinkronkan hanya beberapa folder sebelum pengaturan ulang, Anda harus melakukannya lagi setelah sinkronisasi selesai.</span><span class="sxs-lookup"><span data-stu-id="646aa-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="646aa-123">Baca [memilih folder OneDrive yang akan disinkronkan ke komputer Anda](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   untuk informasi selengkapnya.</span><span class="sxs-lookup"><span data-stu-id="646aa-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="646aa-124">Anda harus menyelesaikan ini untuk OneDrive pribadi dan OneDrive for Business Anda.</span><span class="sxs-lookup"><span data-stu-id="646aa-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>