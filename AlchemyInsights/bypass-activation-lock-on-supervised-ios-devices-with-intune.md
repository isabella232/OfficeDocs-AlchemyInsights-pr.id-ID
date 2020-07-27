---
title: Bypass aktivasi kunci pada perangkat iOS diawasi dengan Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423731"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a>Bypass aktivasi kunci pada perangkat iOS diawasi dengan Intune

Kemampuan untuk melewati kunci aktivasi pada perangkat iOS membuatnya lebih mudah untuk pulih dari skenario di mana pengguna mengaktifkan kunci aktivasi pada perangkat korporat, dan kemudian meninggalkan perusahaan.

Prasyarat untuk melewati kunci aktivasi meliputi:

- Perangkat adalah "diawasi."
- Kunci aktivasi berhasil diaktifkan menggunakan kebijakan pembatasan iOS perangkat di Intune.

Selain itu, ketika melewati kunci aktivasi, Anda harus:

- Fisik memiliki perangkat yang dihapus.
- Salin kode sebelum Anda mengeluarkan penghapusan.

**Catatan:** Kode wipe tidak case sensitive, sehingga karakter "-" tidak diperlukan.

Untuk detailnya, lihat [bypass kunci aktivasi pada perangkat iOS yang diawasi dengan Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).

**FAQ**

Q: **saya mengeluarkan tindakan jauh untuk menghapus data perusahaan dari perangkat, dan sekarang terjebak dalam keadaan tertunda.**

A: untuk tindakan jarak jauh untuk berhasil menyelesaikan, perangkat target harus online dan sehat. Dalam situasi berikut, tindakan jarak jauh tetap dalam keadaan tertunda selama 30 hari, atau sampai perangkat mengakui perintah saat perangkat:

- Tidak memiliki konektivitas.
- Kehilangan status manajemennya dengan Intune.

Jika Anda merasa perangkat tidak lagi dapat memeriksa, dan tidak akan menghapus data perusahaan, pilih Hapus. Menghapus menghapus rekaman perangkat sehingga tidak lagi muncul di Daftar perangkat Intune. Agar perangkat aktif kembali, pengguna harus mendaftarkan ulang perangkat.

T: **mengapa tindakan jarak jauh tertentu tidak tersedia bagi saya untuk digunakan?**

A: tidak semua platform mendukung semua tindakan perangkat jarak jauh. Tindakan jarak jauh berikut ini khusus platform.

- Kunci aktivasi bypass (hanya iOS)
- Mulai segar (khusus Windows)
- Mode hilang (khusus iOS)
- Menemukan perangkat (khusus iOS)
- Mulai ulang (khusus Windows)

Untuk detail selengkapnya tentang setiap tindakan, lihat [tindakan perangkat yang tersedia](https://docs.microsoft.com/intune/device-management#available-device-actions).