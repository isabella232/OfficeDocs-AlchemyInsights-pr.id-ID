---
title: Aturan DLP untuk nomor rekening bank AS tidak berfungsi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 0b5c1fb175275028c56e47080708520fe115fb38
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932538"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>Masalah DLP dengan nomor rekening bank AS

**Penting**: banyak SharePoint online dan OneDrive pelanggan menjalankan aplikasi penting bisnis terhadap layanan yang berjalan di latar belakang. Ini termasuk migrasi konten, pencegahan kehilangan data (DLP), dan solusi pencadangan. Selama waktu yang belum pernah terjadi sebelumnya, kami mengambil langkah untuk memastikan bahwa SharePoint online dan layanan OneDrive tetap sangat tersedia dan dapat diandalkan untuk pengguna yang bergantung pada layanan lebih dari sebelumnya dalam skenario kerja jarak jauh.

Untuk mendukung tujuan ini, kami telah menerapkan batas pelambatan yang lebih ketat pada aplikasi latar belakang (migrasi, DLP dan solusi cadangan) selama jam siang hari kerja. Anda harus mengharapkan bahwa aplikasi ini akan mencapai throughput yang sangat terbatas selama waktu ini. Namun, selama jam malam dan akhir pekan untuk wilayah ini, Layanan akan siap untuk memproses volume permintaan yang jauh lebih tinggi dari aplikasi latar belakang.

**Masalah DLP dengan nomor rekening bank AS**

Apakah Anda mengalami masalah dengan **pencegahan kehilangan data (DLP)** yang tidak berfungsi untuk konten yang berisi **nomor rekening bank AS** saat menggunakan jenis informasi sensitif DLP di O365? Jika demikian, pastikan konten Anda berisi informasi yang diperlukan untuk apa kebijakan DLP Cari ketika dievaluasi.
  
Misalnya, untuk kebijakan **nomor rekening bank AS** yang dikonfigurasi dengan tingkat kepercayaan 85%, berikut dievaluasi dan harus terdeteksi aturan untuk memicu:
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digit

- **[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 digit berturut-turut.

- **[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Tidak, tidak ada checksum

- **[Definisi:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Sebuah kebijakan DLP adalah 75% yakin bahwa hal itu terdeteksi jenis informasi sensitif jika, dalam kedekatan 300 karakter:

  - Ekspresi reguler Regex_usa_bank_account_number menemukan konten yang sesuai dengan pola

  - Kata kunci dari Keyword_usa_Bank_Account ditemukan.

    Sebagai contoh, contoh berikut akan memicu untuk kebijakan **nomor rekening bank AS** : memeriksa akun 78344011

Untuk informasi lebih lanjut tentang apa yang diperlukan untuk **nomor rekening bank AS** untuk terdeteksi untuk konten Anda, lihat bagian berikut dalam artikel ini: [apa jenis informasi sensitif mencari nomor rekening bank AS](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
Menggunakan jenis informasi sensitif internal yang berbeda, lihat artikel berikut untuk informasi tentang apa yang diperlukan untuk jenis lain: [apa jenis informasi sensitif](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for) mencari
  