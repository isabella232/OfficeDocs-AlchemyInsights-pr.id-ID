---
title: Aturan DLP untuk SSN tidak berfungsi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 0b83a858975ffe1bb70f16a7452a13d57dff5340
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932527"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Masalah DLP dengan nomor jaminan sosial

**Penting**: banyak SharePoint online dan OneDrive pelanggan menjalankan aplikasi penting bisnis terhadap layanan yang berjalan di latar belakang. Ini termasuk migrasi konten, pencegahan kehilangan data (DLP), dan solusi pencadangan. Selama waktu yang belum pernah terjadi sebelumnya, kami mengambil langkah untuk memastikan bahwa SharePoint online dan layanan OneDrive tetap sangat tersedia dan dapat diandalkan untuk pengguna yang bergantung pada layanan lebih dari sebelumnya dalam skenario kerja jarak jauh.

Untuk mendukung tujuan ini, kami telah menerapkan batas pelambatan yang lebih ketat pada aplikasi latar belakang (migrasi, DLP dan solusi cadangan) selama jam siang hari kerja. Anda harus mengharapkan bahwa aplikasi ini akan mencapai throughput yang sangat terbatas selama waktu ini. Namun, selama jam malam dan akhir pekan untuk wilayah ini, Layanan akan siap untuk memproses volume permintaan yang jauh lebih tinggi dari aplikasi latar belakang.

**Masalah DLP dengan SSNs**

Apakah Anda mengalami masalah dengan **pencegahan kehilangan data (DLP)** yang tidak berfungsi untuk konten yang berisi **nomor jaminan sosial (SSN)** saat menggunakan jenis informasi sensitif di Office 365? Jika demikian, pastikan konten Anda berisi informasi yang diperlukan untuk apa kebijakan DLP Cari. 
  
Misalnya, untuk kebijakan SSN yang dikonfigurasi dengan tingkat kepercayaan 85%, berikut dievaluasi dan harus terdeteksi untuk aturan untuk memicu:
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digit, yang mungkin dalam pola diformat atau tidak diformat

- **[Pola:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Empat fungsi mencari SSNs dalam empat pola yang berbeda:

  - Func_ssn menemukan SSNs dengan pra-2011 format yang kuat yang diformat dengan tanda hubung atau spasi (DDD-DD-DDDD atau DDD DD DDDD)

  - Func_unformatted_ssn menemukan SSNs dengan pra-2011 format yang kuat yang telah diformat sebagai sembilan digit berturut-turut (ddddddddd)

  - Func_randomized_formatted_ssn menemukan Post-2011 SSNs yang diformat dengan tanda hubung atau spasi (DDD-DD-DDDD atau DDD DD DDDD)

  - Func_randomized_unformatted_ssn menemukan Post-2011 SSNs yang terformat sebagai sembilan digit berturut-turut (ddddddddd)

- **[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Tidak, tidak ada checksum

- **[Definisi:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Sebuah kebijakan DLP adalah 85% yakin bahwa hal itu terdeteksi jenis informasi sensitif jika, dalam kedekatan 300 karakter:

  - [Fungsi Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) menemukan konten yang sesuai dengan pola.

  - Kata kunci dari [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) ditemukan. Contoh kata kunci meliputi: *jaminan sosial, jaminan sosial #, SOC SEC, SSN* . Sebagai contoh, contoh berikut akan memicu kebijakan DLP SSN: **SSN: 489-36-8350**
  
Untuk informasi lebih lanjut tentang apa yang diperlukan untuk SSNs untuk terdeteksi untuk konten Anda, lihat bagian berikut dalam artikel ini: [apa jenis informasi sensitif mencari SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Menggunakan jenis informasi sensitif internal yang berbeda, lihat artikel berikut untuk informasi tentang apa yang diperlukan untuk jenis lain: [apa jenis informasi sensitif](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for) mencari
  