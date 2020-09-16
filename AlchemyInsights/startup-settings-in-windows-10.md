---
title: Pengaturan startup di Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: e49faca66785c6611dda702a381c39cdb10884f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751138"
---
# <a name="startup-settings-in-windows-10"></a>Pengaturan startup di Windows 10

**Mengubah aplikasi yang berjalan secara otomatis pada saat startup**

1. Masuk ke [pengaturan > aplikasi > mulai](ms-settings:startupapps?activationSource=GetHelp).

2. Pastikan semua aplikasi yang ingin Anda **jalankan pada startup diaktifkan.**

**Menambahkan aplikasi untuk dijalankan secara otomatis saat memulai**

1. Klik atau ketuk **mulai** dan temukan aplikasi yang ingin Anda jalankan pada startup.

2. Klik kanan aplikasi, klik **lainnya**, lalu klik **buka lokasi file**. Ini akan membuka lokasi tempat pintasan ke aplikasi disimpan. Jika tidak ada opsi untuk lokasi file yang terbuka, itu berarti aplikasi tidak dapat dijalankan pada startup.

3. Dengan lokasi file terbuka, tekan **tombol logo Windows + R**, ketikkan **Shell: startup**, lalu klik **OK**. Ini akan membuka folder startup.

4. Salin dan tempelkan pintasan ke aplikasi dari lokasi file ke folder startup.

**Opsi startup tingkat lanjut (termasuk mode aman, pengaturan UEFI, dan booting dari perangkat lain)**

1. Simpan pekerjaan Anda dan tutup setiap dokumen yang terbuka, karena langkah-langkah ini akan memulai ulang PC Anda.

2. Buka [pengaturan > perbarui & keamanan > pemulihan](ms-settings:recovery?activationSource=GetHelp).

3. Di bawah **startup tingkat lanjut**, klik **mulai ulang sekarang**. 

4. Setelah PC dimulai ulang ke layar pilih opsi:

    - Untuk boot dari perangkat seperti drive USB, klik **Gunakan perangkat**.

    - Untuk memasukkan pengaturan UEFI (terkadang disebut penyetelan BIOS), klik **pemecahan masalah > opsi tingkat lanjut > UEFI pengaturan firmware**. 

    - Untuk memasukkan mode aman atau mengubah pengaturan startup tingkat lanjut, klik **pemecahan masalah > opsi tingkat lanjut > pengaturan startup**, lalu klik **mulai ulang**. Anda mungkin diminta untuk memasukkan [kunci pemulihan BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key). Setelah PC dimulai ulang lagi, klik Pengaturan mulai yang ingin Anda gunakan.