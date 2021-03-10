---
title: Menerapkan praktik terbaik untuk kueri berburu tingkat lanjut
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694271"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Menerapkan praktik terbaik untuk kueri berburu tingkat lanjut

Untuk mendapatkan hasil lebih cepat dan menghindari waktu tunggu saat menjalankan kueri yang kompleks, Terapkan praktik terbaik ini:

- Saat mencoba kueri baru, selalu gunakan batas untuk menghindari rangkaian hasil yang sangat besar. Juga, gunakan `count` untuk membuat penilaian awal dari ukuran rangkaian hasil.
- Gunakan filter waktu terlebih dahulu. Idealnya, Batasi kueri Anda hingga tujuh hari.
- Di awal kueri, tepat setelah filter waktu, tambahkan filter yang diharapkan untuk menghapus sebagian besar data.
- Saat mencari token penuh, gunakan operator dan `has` bukan `contains` .
- Menjalankan pencarian pada kolom tertentu dan bukan di seluruh kolom.
- Saat bergabung ke tabel, tentukan tabel terlebih dahulu dengan lebih sedikit baris.
- `project` hanya kolom yang diperlukan dari tabel yang sudah Anda ikuti.

Untuk mempelajari selengkapnya, lihat [praktik terbaik kueri berburu lanjutan](https://go.microsoft.com/fwlink/?linkid=2144812).
