---
title: Menemukan perangkat iOS yang hilang dengan Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439628"
---
# <a name="locating-lost-ios-devices-with-intune"></a>Menemukan perangkat iOS yang hilang dengan Intune

Mengaktifkan mode hilang pada perangkat iOS memungkinkan administrator untuk memiliki pesan dan nomor telepon kontak yang ditampilkan pada layar kunci.

Setelah mode hilang diaktifkan admin dapat menggunakan perangkat Cari tindakan untuk mengidentifikasi lokasi fisik perangkat.

Tindakan temukan perangkat di Intune bekerja dengan perangkat iOS untuk menampilkan lokasi perangkat tertentu pada peta.

Menggunakan tindakan ini memerlukan perangkat iOS untuk berada di:

- Mode diawasi
- Mode hilang

Untuk informasi lebih lanjut, lihat [mengaktifkan mode hilang pada perangkat iOS/ipados dengan Intune](https://docs.microsoft.com/intune/device-lost-mode) dan [menemukan perangkat iOS/ipados hilang atau dicuri dengan Intune](https://docs.microsoft.com/intune/device-locate).

**FAQ**

T: saya mengeluarkan tindakan jarak jauh untuk menghapus data perusahaan dari perangkat, dan sekarang terjebak dalam keadaan tertunda.

A: untuk tindakan jarak jauh untuk berhasil menyelesaikan, perangkat target harus online dan sehat. Dalam situasi berikut, tindakan jarak jauh tetap dalam keadaan tertunda selama 30 hari, atau sampai perangkat mengakui perintah:

- Bila perangkat tidak memiliki konektivitas
- Ketika perangkat kehilangan status manajemen dengan Intune

Jika Anda merasa perangkat tidak lagi masuk, dan tidak dapat menghapus data perusahaan, pilih Hapus. Menghapus menghapus rekaman perangkat sehingga tidak lagi muncul di Daftar perangkat Intune. Jika perangkat aktif kembali, pengguna harus mendaftarkannya kembali.

T: Mengapa tindakan jarak jauh tertentu tidak tersedia bagi saya untuk digunakan?

A: tidak semua platform mendukung semua tindakan perangkat jarak jauh. Tindakan jarak jauh berikut ini khusus platform, sehingga tersedia hanya untuk platform yang dicatat.

- Kunci aktivasi bypass (hanya iOS)
- Mulai segar (khusus Windows)
- Mode hilang (khusus iOS)
- Menemukan perangkat (khusus iOS)
- Mulai ulang (khusus Windows)

Untuk detail selengkapnya tentang setiap tindakan, lihat [tindakan perangkat yang tersedia](https://docs.microsoft.com/intune/device-management#available-device-actions).