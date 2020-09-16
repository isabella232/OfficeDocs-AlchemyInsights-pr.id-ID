---
title: Mitigasi kesalahan Aplikasi tidak terdeteksi
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
- "9000171"
- "1712"
ms.openlocfilehash: 498c2ec78bc9f4a7bc7d77d12b488be2cf0bf79a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666981"
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
