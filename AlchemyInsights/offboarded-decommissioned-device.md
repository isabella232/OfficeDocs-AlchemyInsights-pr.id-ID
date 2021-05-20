---
title: Masalah dengan penghapusan perangkat offboarded atau yang dinonaktifkan dari Inventaris Perangkat
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
ms.openlocfilehash: 46ac46c583cd0ac956797737d8150277f0d79ba5
ms.sourcegitcommit: c685f197dbf83a9dfd85e9acfdf14a4daf0e9a5a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/11/2021
ms.locfileid: "52564340"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a>Masalah dengan penghapusan perangkat offboarded atau yang dinonaktifkan dari Inventaris Perangkat

Pertahanan Microsoft untuk Titik Akhir saat ini tidak mengizinkan penghapusan catatan perangkat dari perangkat offboarded atau yang dinonaktifkan secara manual dari Inventaris Perangkat.

Untuk tujuan keamanan, perangkat tetap ada di portal sebagai catatan riwayat hingga 180 hari. Namun, data perangkat di purged sesuai dengan periode penyimpanan yang dikonfigurasi.

**Catatan:** Perangkat yang dinonaktifkan atau offboarded akan beralih secara otomatis ke **keadaan Tidak** Aktif setelah tujuh hari. Selain itu, perangkat yang tidak aktif dalam 30 hari terakhir tidak difleksikan ke dalam data yang mencerminkan Pengelolaan Ancaman dan Kerentanan skor paparan atau Microsoft Secure Score untuk Perangkat.
 
Jika anda masih tidak ingin melihat perangkat tertentu dalam tampilan Inventaris Perangkat, coba tempatkan tag perangkat untuk memfilter perangkat yang dinonaktifkan dari tampilan Inventaris Perangkat.

Untuk informasi selengkapnya, lihat:

[Perangkat offboard dari Pertahanan Microsoft untuk layanan Titik Akhir](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[Skor paparan di Pengelolaan Ancaman dan Kerentanan](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[Memperbaiki sensor yang tidak sehat di Pertahanan Microsoft untuk Titik Akhir](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[Cara menggunakan penandaan secara efektif (Bagian 1)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[Cara menggunakan penandaan secara efektif (Bagian 2)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[Cara menggunakan penandaan secara efektif (Bagian 3)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




