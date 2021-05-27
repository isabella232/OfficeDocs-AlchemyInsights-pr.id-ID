---
title: Inventaris perangkat lunak hilang atau tidak akurat
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/26/2021
ms.locfileid: "52676518"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a>Inventaris perangkat lunak hilang atau tidak akurat

Inventaris perangkat lunak di Pengelolaan Ancaman dan Kerentanan (TVM) adalah daftar perangkat lunak yang dikenal di organisasi Anda dengan Common Platform Enumerations (CPE) resmi.

Produk perangkat lunak tanpa CPE resmi tidak memiliki kerentanan yang diterbitkan. Inventaris juga menyertakan detail seperti nama vendor, jumlah item, ancaman, dan jumlah perangkat yang diekspos.

Perubahan perangkat lunak pada perangkat biasanya terlihat di portal keamanan dalam waktu dua jam. Namun, terkadang membutuhkan waktu lebih lama. Saat ini, sinkronisasi belum dapat dilakukan; ini adalah penilaian berkelanjutan yang sedang berlangsung.

Jika Anda membuat perubahan perangkat lunak dan perubahan tersebut tidak secara akurat terlihat di TVM setelah 5 jam, ikuti langkah-langkah berikut:

1. Periksa bagian bukti perangkat lunak untuk memahami bagaimana perangkat lunak terdeteksi.
1. Pastikan bahwa perangkat lunak ini didukung. Perangkat lunak mungkin hanya terlihat di tingkat perangkat meskipun saat ini tidak didukung oleh Pengelolaan Ancaman dan Kerentanan. Namun, hanya data terbatas yang tersedia.
1. Untuk langkah-langkah melaporkan ketidakakuratan dari portal, lihat [Melaporkan ketidakakuratan](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).
   
    **Catatan**: Melaporkan ketidakakuratan dari portal MDE adalah saluran satu arah yang harus di engineering. Jika masalah mendesak, buka tiket dukungan.

Untuk informasi selengkapnya, lihat [Inventaris perangkat lunak - Pengelolaan Ancaman dan Kerentanan](/microsoft-365/security/defender-endpoint/tvm-software-inventory).