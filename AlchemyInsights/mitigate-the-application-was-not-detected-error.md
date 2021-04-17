---
title: Mitigasi kesalahan Aplikasi tidak terdeteksi
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
- "9000171"
- "1712"
ms.openlocfilehash: 4e0599f9bdf2c7d16d009627f44b3691c2c250b7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836354"
---
# <a name="mitigate-the-application-was-not-detected-error"></a>Mitigasi kesalahan "Aplikasi tidak terdeteksi"

Kesalahan penginstalan aplikasi, “Aplikasi tidak terdeteksi setelah penginstalan berhasil diselesaikan,” dilaporkan oleh Intune, mungkin terjadi di semua platform OS utama (Windows, iOS, dan Android).

Skenario paling umum yang menghasilkan kesalahan ini mencakup:

- Aplikasi telah diperbarui di luar Intune (dari bursa aplikasi pihak ketiga) setelah penyebaran awal. Misalnya, beberapa aplikasi seperti Google Chrome mungkin menjalankan pembaruan otomatis.
- Pengguna telah menghapus instalan aplikasi setelah penginstalan awal.

Untuk memitigasi masalah ini, lakukan peninjauan terlebih dahulu terhadap perangkat yang terpengaruh guna menentukan skenario terjadinya kesalahan.

- Jika aplikasi telah diperbarui di luar Intune, penyebaran aplikasi dapat diatur untuk mengabaikan versi aplikasi. Untuk melakukannya, di bawah **Konfigurasi Aplikasi > Informasi Aplikasi**, atur **Abaikan Versi Aplikasi** ke **Ya**.
- Saat menargetkan klien, mungkin tepat untuk menyebarkan aplikasi sebagai “diperlukan,” dan untuk memastikan bahwa versi terbaru disebarkan.
- Alternatifnya, di platform iOS, dimungkinkan untuk menggunakan fungsi **autoupdate** yang terkait dengan Program Pembelian Volume Apple, yang dapat dikonfigurasi agar secara otomatis memperbarui ke versi aplikasi baru saat tersedia.

Untuk informasi selengkapnya tentang pemecahan masalah penginstalan aplikasi, silakan lihat [Memecahkan masalah penginstalan aplikasi](https://docs.microsoft.com/intune/troubleshoot-app-install).
