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
# <a name="troubleshoot-onedrive-crashes"></a>Memecahkan masalah OneDrive crash

Jika OneDrive berulang kali mengalami crash, coba langkah pemecahan masalah ini:

**Pastikan kunci registri tidak diatur:**

1. Menggunakan editor registri, navigasikan ke HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive
2. Jika DisableFileSyncNGSC ada dan disetel ke 1, buka kunci dan Ubah nilainya ke 0.
3. Luncurkan OneDrive secara manual dengan masuk ke mulai ![Tekan tombol Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), ketikkan OneDrive dalam kotak pencarian, lalu klik aplikasi desktop OneDrive.

**Atur ulang OneDrive:**

Catatan

- Mereset OneDrive memutus semua koneksi sinkronisasi yang ada (termasuk OneDrive pribadi jika disetel).
- Anda tidak akan kehilangan file atau data dengan mengatur ulang OneDrive di komputer Anda.

**Untuk mengatur ulang OneDrive:**

1. Buka dialog jalankan dengan menekan tombol Windows dan R.
2. Ketikkan% localappdata% \Microsoft\OneDrive\onedrive.exe/reset dan tekan OK. Jendela perintah mungkin muncul sebentar.
3. Luncurkan OneDrive secara manual dengan masuk ke mulai ![Tekan tombol Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), ketikkan OneDrive dalam kotak pencarian, lalu klik aplikasi desktop OneDrive.

Catatan

- Jika Anda telah memilih untuk menyinkronkan hanya beberapa folder sebelum pengaturan ulang, Anda harus melakukannya lagi setelah sinkronisasi selesai. Baca [memilih folder OneDrive yang akan disinkronkan ke komputer Anda](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   untuk informasi selengkapnya.
- Anda harus menyelesaikan ini untuk OneDrive pribadi dan OneDrive for Business Anda.