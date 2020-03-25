---
title: Aturan DLP untuk nomor kartu kredit tidak berfungsi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932446"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Masalah DLP dengan nomor kartu kredit

**Penting**: banyak SharePoint online dan OneDrive pelanggan menjalankan aplikasi penting bisnis terhadap layanan yang berjalan di latar belakang. Ini termasuk migrasi konten, pencegahan kehilangan data (DLP), dan solusi pencadangan. Selama waktu yang belum pernah terjadi sebelumnya, kami mengambil langkah untuk memastikan bahwa SharePoint online dan layanan OneDrive tetap sangat tersedia dan dapat diandalkan untuk pengguna yang bergantung pada layanan lebih dari sebelumnya dalam skenario kerja jarak jauh.

Untuk mendukung tujuan ini, kami telah menerapkan batas pelambatan yang lebih ketat pada aplikasi latar belakang (migrasi, DLP dan solusi cadangan) selama jam siang hari kerja. Anda harus mengharapkan bahwa aplikasi ini akan mencapai throughput yang sangat terbatas selama waktu ini. Namun, selama jam malam dan akhir pekan untuk wilayah ini, Layanan akan siap untuk memproses volume permintaan yang jauh lebih tinggi dari aplikasi latar belakang.

**Masalah DLP dengan nomor kartu kredit**

Apakah Anda mengalami masalah dengan **pencegahan kehilangan data (DLP)** tidak bekerja untuk konten yang berisi **nomor kartu kredit** saat menggunakan jenis informasi sensitif DLP di O365? Jika demikian, pastikan konten Anda berisi informasi yang diperlukan untuk memicu kebijakan DLP ketika dievaluasi. Misalnya, untuk **kebijakan kartu kredit** yang dikonfigurasi dengan tingkat kepercayaan 85%, berikut dievaluasi dan harus terdeteksi untuk aturan untuk memicu:
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digit yang dapat diformat atau belum diformat (dddddddddddddddd) dan harus lulus tes Luhn.

- **[Pola:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Pola yang sangat kompleks dan kuat yang mendeteksi kartu dari semua merek utama di seluruh dunia, termasuk Visa, MasterCard, Discover Card, JCB, American Express, kartu hadiah, dan kartu restoran.

- **[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Ya, checksum Luhn

- **[Definisi:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Sebuah kebijakan DLP adalah 85% yakin bahwa hal itu terdeteksi jenis informasi sensitif jika, dalam kedekatan 300 karakter:

  - Fungsi Func_credit_card menemukan konten yang sesuai dengan pola.

  - Salah satu dari berikut ini benar:

  - Kata kunci dari Keyword_cc_verification ditemukan.

  - Kata kunci dari Keyword_cc_name ditemukan

  - Fungsi Func_expiration_date menemukan tanggal dalam format tanggal yang tepat.

  - Checksum lolos

    Sebagai contoh, contoh berikut akan memicu untuk kebijakan nomor kartu kredit DLP:

  - Visa: 4485 3647 3952 7352
  
  - Berakhir: 2/2009

Untuk informasi lebih lanjut tentang apa yang diperlukan untuk **nomor kartu kredit** akan terdeteksi untuk konten Anda, lihat bagian berikut dalam artikel ini: [apa jenis informasi sensitif mencari kartu kredit #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Menggunakan jenis informasi sensitif internal yang berbeda, lihat artikel berikut untuk informasi tentang apa yang diperlukan untuk jenis lain: [apa jenis informasi sensitif](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for) mencari
  