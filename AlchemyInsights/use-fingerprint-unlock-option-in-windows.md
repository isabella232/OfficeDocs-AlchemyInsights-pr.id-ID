---
title: Gunakan opsi Buka kunci sidik jari di Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 8a5059c722c306ad79811140062cec7f52f31766
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588319"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Gunakan opsi Buka kunci sidik jari di Windows 10

**Mengaktifkan Windows Hello Fingerprint**

Untuk membuka Windows 10 menggunakan sidik jari Anda, Anda perlu mengatur Windows Hello Fingerprint dengan menambahkan (membiarkan Windows belajar mengenali) setidaknya satu jari. 

1. Buka **pengaturan > akun > opsi masuk** (atau klik [di sini](ms-settings:signinoptions?activationSource=GetHelp)). Opsi masuk yang tersedia akan dicantumkan. Misalnya:

    ![Opsi masuk.](media/sign-in-options.png)

2. Klik atau ketuk **Windows Halo sidik jari**, lalu klik **Siapkan**. Di jendela penyiapan Windows Hello, klik **mulai**. Sensor sidik jari akan aktif, dan Anda akan diminta untuk menempatkan jari Anda pada sensor:

   ![Sensor sidik jari.](media/fingerprint-sensor.png)

3. Ikuti petunjuk yang akan meminta Anda untuk memindai jari secara berulang-ulang. Setelah ini selesai, Anda akan memiliki opsi untuk menambahkan jari lain yang mungkin ingin Anda gunakan untuk masuk. Lain kali Anda masuk ke Windows 10, Anda akan memiliki pilihan untuk menggunakan sidik jari Anda untuk melakukannya.

**Windows Halo sidik jari tidak tersedia sebagai Opsi masuk**

Jika Windows Halo sidik jari tidak ditampilkan sebagai pilihan dalam **sign-in pilihan**, itu berarti Windows tidak menyadari setiap sidik jari pembaca/scanner MELEKAT pada PC Anda, atau bahwa kebijakan sistem mencegah penggunaannya (jika misalnya PC Anda dikelola oleh tempat kerja Anda). Untuk memecahkan masalah: 

1. Pilih tombol **mulai** di taskbar dan Cari **Device Manager**.

2. Klik atau ketuk untuk membuka **pengelola perangkat**.

3. Pada pengelola perangkat, Perluas perangkat biometrik dengan mengeklik Chevron-nya.

   ![Perangkat biometrik.](media/biometric-devices.png)

4. Pemindai sidik jari Anda harus terdaftar sebagai perangkat biometrik, seperti pemindai WBDI Synaptics:

   ![Perangkat biometrik.](media/biometric-devices-expanded.png)

5. Jika pemindai sidik jari Anda tidak ditampilkan, dan pemindai diintegrasikan ke dalam PC Anda, buka situs web produsen PC. Di bagian dukungan teknis untuk model PC Anda, Cari Driver Windows 10 untuk pemindai yang dapat Anda instal.

6. Jika pemindai terpisah dari PC (terpasang melalui USB), buka situs web produsen pemindai untuk menemukan dan menginstal perangkat lunak pengandar perangkat Windows 10 untuk model pemindai yang Anda miliki.
