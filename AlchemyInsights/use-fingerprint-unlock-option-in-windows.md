---
title: Menggunakan opsi buka kunci sidik jari Windows 10
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
ms.openlocfilehash: a171d889705a0035981465bdaa5a8f07b9d2eb7200ba4c948f2aaccbf2cc0a21
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971938"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Menggunakan opsi buka kunci sidik jari Windows 10

**Mengaktifkan Windows Hello Sidik Jari**

Untuk membuka Windows 10 jari Anda, siapkan sidik jari Windows Hello sidik jari dengan menambahkan (memungkinkan Windows belajar mengenali) setidaknya satu jari. 

1. Masuk ke **Pengaturan > Akun > opsi Masuk (atau** klik di [sini](ms-settings:signinoptions?activationSource=GetHelp)). Opsi masuk yang tersedia akan dicantumkan. Misalnya:

    ![Opsi masuk.](media/sign-in-options.png)

2. Klik atau ketuk **Windows Hello Sidik** Jari, lalu **klik Siapkan.** Di Windows Hello penyiapan Anda, **klik Mulai.** Sensor sidik jari akan aktif, dan Anda akan diminta untuk menempatkan jari di sensor:

   ![Sensor sidik jari.](media/fingerprint-sensor.png)

3. Ikuti instruksi, yang akan meminta Anda untuk memindai jari berulang kali. Setelah ini selesai, Anda akan memiliki opsi untuk menambahkan jari lain yang mungkin ingin Anda gunakan untuk masuk. Pada kali berikutnya Anda masuk Windows 10, Anda akan memiliki opsi untuk menggunakan sidik jari Anda.

**Windows Hello Sidik jari tidak tersedia sebagai opsi masuk**

Jika Windows Hello Sidik Jari tidak diperlihatkan sebagai opsi masuk **,** artinya Windows tidak mengetahui pembaca/pemindai sidik jari apa pun yang terhubung ke PC Anda, atau bahwa kebijakan sistem mencegah penggunaannya (jika PC Anda dikelola oleh tempat kerja Anda). Untuk memecahkan masalah: 

1. Pilih **tombol** Mulai di Taskbar, lalu cari **Manajer Perangkat.**

2. Klik atau ketuk untuk membuka **Manajer Perangkat.**

3. Di Manajer Perangkat, perluas perangkat Biometrik dengan mengklik chevronnya.

   ![Perangkat biometrik.](media/biometric-devices.png)

4. Pemindai sidik jari Anda akan tercantum sebagai perangkat biometrik, seperti pemindai WBDI Synaptics:

   ![Perangkat biometrik.](media/biometric-devices-expanded.png)

5. Jika pemindai sidik jari Anda tidak terlihat, dan pemindai terintegrasi dengan PC Anda, masuk ke situs web pabrikan PC. Di bagian dukungan teknis untuk model PC Anda, cari driver Windows 10 untuk pemindai yang bisa Anda instal.

6. Jika pemindai terpisah dari PC (dilampirkan melalui USB), masuk ke situs web produsen pemindai untuk menemukan dan menginstal perangkat lunak driver Windows 10 untuk model pemindai yang Anda miliki.
