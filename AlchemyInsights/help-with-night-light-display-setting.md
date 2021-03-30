---
title: Bantuan terkait pengaturan tampilan cahaya malam
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
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404664"
---
# <a name="help-with-the-night-light-display-setting"></a>Bantuan terkait pengaturan tampilan cahaya malam

Untuk mempelajari selengkapnya tentang pengaturan tampilan waktu malam, [lihat Mengatur tampilan Anda untuk waktu malam di Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).

Jika opsi cahaya malam berwarna abu-abu di Pengaturan, periksa driver tampilan Anda: 

1. Klik kotak pencarian di taskbar Anda dan ketik **Manajer Perangkat**, lalu pilih **Manajer Perangkat** di hasil pencarian.
1. Perluas **Adaptor tampilan**. 

Sayangnya, fitur cahaya malam tidak tersedia jika perangkat Anda menggunakan driver DisplayLink atau driver Tampilan Dasar.

Fitur cahaya malam menggunakan teknologi grafik terbaru, sehingga Anda mungkin perlu memperbarui driver tampilan:  

- Periksa pembaruan dengan masuk ke Mulai  >  **Pengaturan**  >  **Pembaruan & Windows**  >  **Update** Periksa  >  **Pembaruan Windows.**  

ATAU

- Kunjungi situs web dukungan produsen perangkat keras Anda untuk mengunduh dan menginstal driver tampilan terbaru secara manual.

## <a name="reset-night-light-in-the-registry"></a>Mengatur ulang cahaya malam di registri

Jika memperbarui driver tampilan tidak berfungsi, Anda mungkin perlu mengatur ulang lampu malam dalam registri.  

**Perhatian:** Langkah pemecahan masalah ini disarankan hanya untuk pengguna tingkat lanjut. Masalah serius dapat terjadi jika Anda salah mengubah registri. Untuk perlindungan tambahan, buat cadangan registri sebelum mengubahnya agar Anda dapat memulihkannya jika terjadi masalah.

1. Dalam kotak pencarian, ketikkan **regedit**, lalu pilih **Editor Registri** dalam hasil pencarian.

1. Masuk ke kunci registri berikut: 

    HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount

1. Ekspor lalu hapus subkey berikut:$$windows.data.bluelightreduction.bluelightreductionstate

1. Ekspor lalu hapus subkey berikut:$$windows.data.bluelightreduction.settings

1. Mulai ulang Windows dan pastikan apakah opsi cahaya malam tersedia.


