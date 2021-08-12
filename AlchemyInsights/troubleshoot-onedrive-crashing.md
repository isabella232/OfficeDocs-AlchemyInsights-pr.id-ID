---
title: Memecahkan OneDrive masalah crash
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
ms.openlocfilehash: d5982bafbb8aaa1d240a34c071efe37e92c2ec5c5170dc59337df9a5435e22e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53921010"
---
# <a name="troubleshoot-onedrive-crashes"></a>Memecahkan OneDrive masalah crash

Jika OneDrive crash berulang kali, cobalah langkah-langkah pemecahan masalah ini:

**Pastikan kunci registri tidak diatur:**

1. Menggunakan Editor Registri, navigasikan ke HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Jika DisableFileSyncNGSC ada dan diatur ke 1, buka kunci dan ubah nilai ke 0.
3. Luncurkan OneDrive secara manual dengan membuka Mulai ![Tekan tombol Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), OneDrive dalam kotak pencarian, lalu klik aplikasi desktop OneDrive Anda.

**Reset OneDrive:**

Catatan:

- Mengatur ulang OneDrive memutuskan semua koneksi sinkronisasi yang ada (termasuk koneksi OneDrive pribadi jika disiapkan).
- Anda tidak akan kehilangan file atau data dengan mengatur ulang OneDrive komputer.

**Untuk mereset OneDrive:**

1. Buka dialog Jalankan dengan menekan Windows dan R.
2. Ketik %localappdata%\Microsoft\OneDrive\onedrive.exe /reset, lalu tekan OK. Jendela Perintah mungkin akan muncul sebentar.
3. Luncurkan OneDrive secara manual dengan membuka Mulai ![Tekan tombol Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), OneDrive dalam kotak pencarian, lalu klik aplikasi desktop OneDrive Anda.

Catatan:

- Jika memilih untuk menyinkronkan beberapa folder saja sebelum mengatur ulang, Anda perlu melakukannya lagi setelah sinkronisasi selesai. Baca [Memilih folder OneDrive mana yang disinkronkan ke komputer Anda](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)untuk informasi   selengkapnya.
- Anda harus menyelesaikan ini untuk alamat email atau OneDrive OneDrive for Business.