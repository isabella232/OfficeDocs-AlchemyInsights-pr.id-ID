---
title: Menerapkan praktik terbaik untuk kueri pencarian tingkat lanjut
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
ms.openlocfilehash: e2a22563a840cd6017afd343bad108be216738742938a48ba5ceb1010fd16098
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930136"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Menerapkan praktik terbaik untuk kueri pencarian tingkat lanjut

Untuk mendapatkan hasil lebih cepat dan menghindari waktu habis saat menjalankan kueri kompleks, terapkan praktik terbaik ini:

- Saat mencoba kueri baru, selalu gunakan batasan, untuk menghindari mendapatkan kumpulan hasil yang sangat besar. Selain itu, `count` gunakan untuk membuat penilaian awal tentang ukuran kumpulan hasil.
- Gunakan filter waktu terlebih dahulu. Idealnya, batasi kueri Anda hingga tujuh hari.
- Di awal kueri, tepat setelah filter waktu, tambahkan filter yang diharapkan untuk menghapus sebagian besar data.
- Ketika mencari token lengkap, gunakan `has` operator dan bukan `contains` .
- Jalankan pencarian pada kolom tertentu dan bukan di seluruh kolom.
- Ketika menggabungkan tabel, pertama-dulu tentukan tabel dengan baris yang lebih sedikit.
- `project` hanya kolom yang diperlukan dari tabel yang sudah Anda ikuti.

Untuk mempelajari selengkapnya, lihat [Praktik terbaik kueri pencarian tingkat lanjut.](https://go.microsoft.com/fwlink/?linkid=2144812)
