---
title: Masalah dengan menghapus perangkat yang tidak papan atau dinonaktifkan dari Inventaris Perangkat
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 6eb59d16a1dab2de0e7a44faf9b34be6432342f9e20c94b6932e69e937751add
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/11/2021
ms.locfileid: "57892006"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a>Masalah dengan menghapus perangkat yang tidak papan atau dinonaktifkan dari Inventaris Perangkat

Pertahanan Microsoft untuk Titik Akhir saat ini tidak mengizinkan penghapusan catatan perangkat dari perangkat offboarded atau pennonaktifkan secara manual dari Inventaris Perangkat.

Untuk tujuan keamanan, perangkat tetap ada di portal sebagai catatan riwayat hingga 180 hari. Namun, data perangkat di purged sesuai dengan periode penyimpanan yang dikonfigurasi.

**Catatan:** Perangkat yang dinonaktifkan atau offboarded akan beralih secara otomatis ke **keadaan Tidak** Aktif setelah tujuh hari. Selain itu, perangkat yang tidak aktif dalam 30 hari terakhir tidak difleksikan ke dalam data yang mencerminkan Pengelolaan Ancaman dan Kerentanan atau Microsoft Secure Score untuk Perangkat.
 
Jika masih tidak ingin melihat perangkat tertentu dalam tampilan Inventaris Perangkat, coba tempatkan tag perangkat untuk memfilter perangkat yang dinonaktifkan dari tampilan Inventaris Perangkat.

Untuk informasi selengkapnya, lihat:

[Perangkat offboard dari Pertahanan Microsoft untuk layanan Titik Akhir](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/offboard-machines.md)

[Skor paparan di Pengelolaan Ancaman dan Kerentanan](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[Memperbaiki sensor yang tidak sehat di Pertahanan Microsoft untuk Titik Akhir](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[Cara menggunakan penandaan secara efektif (Bagian 1)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[Cara menggunakan penandaan secara efektif (Bagian 2)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[Cara menggunakan penandaan secara efektif (Bagian 3)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




