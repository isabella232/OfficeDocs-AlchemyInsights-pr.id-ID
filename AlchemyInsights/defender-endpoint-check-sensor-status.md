---
title: Pemeriksa Titik Akhir Pertahanan memeriksa status sensor
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676177"
---
# <a name="defender-endpoint-check-sensor-status"></a>Pemeriksa Titik Akhir Pertahanan memeriksa status sensor

Petak **Perangkat dengan masalah sensor** berada di dasbor Operasi Keamanan. Ubin ini menyediakan informasi dalam kemampuan perangkat individu untuk menyediakan data sensor dan berkomunikasi dengan Pertahanan untuk layanan Titik Akhir. Laporan ini melaporkan berapa banyak perangkat yang memerlukan perhatian dan membantu Anda mengidentifikasi perangkat yang bermasalah dan mengambil tindakan untuk memperbaiki masalah yang diketahui.

Dua indikator status pada ubin memberikan informasi tentang jumlah perangkat yang tidak melaporkan dengan benar ke layanan:

- **Salah konfigurasikan** Perangkat yang mungkin sebagian melaporkan data sensor ke Pertahanan untuk layanan Titik Akhir dan mungkin memiliki kesalahan konfigurasi yang perlu diperbaiki.
- **Tidak Aktif** Perangkat yang telah berhenti melaporkan ke layanan Pertahanan untuk Titik Akhir selama lebih dari tujuh hari dalam sebulan terakhir.

Mengklik salah satu grup mengarahkan Anda ke daftar Perangkat, difilter menurut pilihan Anda. Pada daftar Perangkat, Anda bisa memfilter daftar status kesehatan dengan status berikut ini:

- **Aktif** Perangkat yang secara aktif melaporkan ke Pertahanan untuk layanan Titik Akhir.
- **Salah konfigurasikan** Perangkat yang mungkin sebagian melaporkan data sensor ke Pertahanan untuk layanan Titik Akhir tetapi memiliki kesalahan konfigurasi yang perlu diperbaiki. Perangkat yang dikonfigurasi dengan tidak benar dapat memiliki satu atau kombinasi masalah berikut ini:

    - Tidak ada data sensor - Perangkat telah berhenti mengirim data sensor. Peringatan terbatas dapat dipicu dari perangkat.
    - Komunikasi yang terganggu - Kemampuan untuk berkomunikasi dengan perangkat mengalami gangguan. Mengirim file untuk analisis mendalam, memblokir file, memisahkan perangkat dari jaringan, dan tindakan lain yang memerlukan komunikasi dengan perangkat mungkin tidak berfungsi.
- **Tidak Aktif** Perangkat yang telah berhenti melaporkan ke Layanan Pertahanan untuk Titik Akhir.

Anda dapat mengunduh seluruh daftar dalam format CSV menggunakan fitur Ekspor.

Untuk informasi selengkapnya, lihat [Memeriksa status kesehatan sensor di Pertahanan Microsoft untuk Titik Akhir.](/microsoft-365/security/defender-endpoint/check-sensor-status)

Untuk informasi selengkapnya tentang hal yang menyebabkan perangkat tidak aktif atau salah konfigurasikan, lihat Memperbaiki sensor yang tidak sehat di [Pertahanan Microsoft untuk Titik Akhir.](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)
