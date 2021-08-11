---
title: Pengaturan mulai di Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: 526b92013f26675b5bf42077271ae7dc7003af31fa8f605d76aea92e0ccabfa1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53909829"
---
# <a name="startup-settings-in-windows-10"></a>Pengaturan mulai di Windows 10

**Mengubah aplikasi mana yang berjalan secara otomatis saat startup**

1. Masuk ke [Pengaturan > Aplikasi > Startup](ms-settings:startupapps?activationSource=GetHelp).

2. Pastikan setiap aplikasi yang ingin Anda jalankan saat startup diaktifkan **ke On**.

**Tambahkan aplikasi untuk berjalan secara otomatis saat startup**

1. Klik atau ketuk **Mulai** dan temukan aplikasi yang ingin Anda jalankan saat memulai.

2. Klik kanan aplikasi, klik **Lainnya**, lalu klik **Buka lokasi file.** Tindakan ini akan membuka lokasi tempat pintasan ke aplikasi disimpan. Jika tidak ada opsi untuk Buka lokasi file, artinya aplikasi tidak dapat berjalan saat startup.

3. Dengan lokasi file yang terbuka, tekan **tombol Windows + R**, ketik **shell:startup**, lalu klik **OK.** Ini membuka folder Startup.

4. Salin dan tempel pintasan ke aplikasi dari lokasi file ke folder Startup.

**Opsi mulai tingkat lanjut (termasuk Brankas Mode, pengaturan UEFI, dan booting dari perangkat lain)**

1. Simpan pekerjaan dan tutup dokumen apa pun yang terbuka, karena langkah-langkah ini akan menghidupkan ulang PC Anda.

2. Masuk ke [Pengaturan > Pembaruan & Pemulihan > Anda.](ms-settings:recovery?activationSource=GetHelp)

3. Di **bawah Mulai ulang** tingkat lanjut, klik Mulai ulang **sekarang.** 

4. Setelah PC dihidupkan ulang ke layar Pilih opsi:

    - Untuk melakukan boot dari perangkat seperti drive USB, **klik Gunakan perangkat**.

    - Untuk memasukkan pengaturan UEFI (kadang disebut penyetelan EFE), klik **Pecahkan > Tingkat Lanjut > Firmware UEFI Pengaturan.** 

    - Untuk masuk ke Mode Brankas atau mengubah pengaturan mulai tingkat lanjut, klik Memecahkan > Opsi tingkat **lanjut > Tingkat** Lanjut Pengaturan , lalu klik Mulai **Ulang.** Anda mungkin diminta untuk memasukkan kunci [pemulihan BitLocker Anda.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key) Setelah PC Anda dihidupkan ulang lagi, klik pengaturan mulai yang ingin Anda gunakan.