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
# <a name="troubleshoot-onedrive-crashes"></a>Memecahkan masalah OneDrive lumpuh

Jika OneDrive berulang kali lumpuh, cobalah langkah pemecahan masalah berikut:

**Pastikan kunci registri tidak ditetapkan:**

1. Menggunakan Penyunting registri, navigasikan ke HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive
2. Jika DisableFileSyncNGSC ada dan disetel ke 1, buka kunci dan mengubah nilai ke 0.
3. Secara manual meluncurkan OneDrive dengan pergi ke Start ![Tekan tombol Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), ketik OneDrive di kotak pencarian, dan kemudian klik pada aplikasi OneDrive desktop.

**Setel ulang OneDrive:**

Catatan:

- Mengatur ulang OneDrive terputus semua koneksi sinkronisasi yang ada (termasuk OneDrive pribadi Anda jika disiapkan).
- Anda tidak akan kehilangan file atau data dengan menyetel ulang OneDrive pada komputer Anda.

**Untuk me-reset OneDrive:**

1. Buka dialog jalankan dengan menekan tombol Windows dan R.
2. Ketik% localappdata% \Microsoft\OneDrive\onedrive.exe/reset dan tekan OK. Jendela perintah akan muncul sebentar.
3. Secara manual meluncurkan OneDrive dengan pergi ke Start ![Tekan tombol Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), ketik OneDrive di kotak pencarian, dan kemudian klik pada aplikasi OneDrive desktop.

Catatan:

- Jika Anda telah memilih untuk melakukan sinkronisasi hanya beberapa folder sebelum reset, Anda akan perlu untuk melakukan itu lagi setelah sinkronisasi selesai. Baca [memilih folder OneDrive yang akan disinkronkan ke komputer Anda](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   untuk informasi lebih lanjut.
- Anda akan perlu untuk melengkapi ini untuk OneDrive pribadi Anda dan OneDrive untuk bisnis.