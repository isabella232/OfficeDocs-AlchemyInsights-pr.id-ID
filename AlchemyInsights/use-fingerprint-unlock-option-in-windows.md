---
title: Menggunakan opsi buka kunci sidik jari di Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796680"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Menggunakan opsi buka kunci sidik jari di Windows 10

**Mengaktifkan Sidik Jari Windows Hello**

Untuk membuka kunci Windows 10 menggunakan sidik jari, Anda perlu menyiapkan Sidik Jari Windows Hello dengan menambahkan (memungkinkan Windows mempelajari cara mengenali) setidaknya satu jari. 

1. Masuk ke **Pengaturan > Akun > opsi Masuk (atau** klik di [sini](ms-settings:signinoptions?activationSource=GetHelp)). Opsi masuk yang tersedia akan dicantumkan. Misalnya:

    ![Opsi masuk.](media/sign-in-options.png)

2. Klik atau ketuk **Sidik Jari Windows Hello,** lalu **klik Siapkan.** Di jendela penyiapan Windows Hello, **klik Mulai**. Sensor sidik jari akan aktif, dan Anda akan diminta untuk menempatkan jari di sensor:

   ![Sensor sidik jari.](media/fingerprint-sensor.png)

3. Ikuti instruksi, yang akan meminta Anda untuk memindai jari berulang kali. Setelah ini selesai, Anda akan memiliki opsi untuk menambahkan jari lain yang mungkin ingin Anda gunakan untuk masuk. Pada kali berikutnya masuk ke Windows 10, Anda akan memiliki opsi untuk menggunakan sidik jari Anda.

**Sidik Jari Windows Hello tidak tersedia sebagai opsi masuk**

Jika Sidik Jari Windows Hello tidak diperlihatkan sebagai opsi Masuk **,** artinya Windows tidak mengetahui pembaca/pemindai sidik jari apa pun yang terhubung ke PC Anda, atau bahwa kebijakan sistem mencegah penggunaannya (jika misalnya PC Anda dikelola oleh tempat kerja Anda). Untuk memecahkan masalah: 

1. Pilih **tombol** Mulai di Taskbar, lalu cari **Manajer Perangkat.**

2. Klik atau ketuk untuk membuka **Manajer Perangkat.**

3. Di Manajer Perangkat, perluas perangkat Biometrik dengan mengklik chevronnya.

   ![Perangkat biometrik.](media/biometric-devices.png)

4. Pemindai sidik jari Anda akan tercantum sebagai perangkat biometrik, seperti pemindai WBDI Synaptics:

   ![Perangkat biometrik.](media/biometric-devices-expanded.png)

5. Jika pemindai sidik jari Anda tidak terlihat, dan pemindai terintegrasi dengan PC Anda, masuk ke situs web pabrikan PC. Di bagian dukungan teknis untuk model PC Anda, cari driver Windows 10 untuk pemindai yang dapat diinstal.

6. Jika pemindai terpisah dari PC (dilampirkan melalui USB), masuk ke situs web produsen pemindai untuk menemukan dan menginstal perangkat lunak driver perangkat Windows 10 untuk model pemindai yang Anda miliki.
