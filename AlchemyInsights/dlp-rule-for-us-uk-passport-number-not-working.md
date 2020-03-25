---
title: Aturan DLP untuk US/Inggris paspor nomor tidak bekerja
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c63e814059c897531109aa78725e9811b311fb27
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931265"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Masalah dengan DLP-US/Inggris nomor paspor

**Penting**: banyak SharePoint online dan OneDrive pelanggan menjalankan aplikasi penting bisnis terhadap layanan yang berjalan di latar belakang. Ini termasuk migrasi konten, pencegahan kehilangan data (DLP), dan solusi pencadangan. Selama waktu yang belum pernah terjadi sebelumnya, kami mengambil langkah untuk memastikan bahwa SharePoint online dan layanan OneDrive tetap sangat tersedia dan dapat diandalkan untuk pengguna yang bergantung pada layanan lebih dari sebelumnya dalam skenario kerja jarak jauh.

Untuk mendukung tujuan ini, kami telah menerapkan batas pelambatan yang lebih ketat pada aplikasi latar belakang (migrasi, DLP dan solusi cadangan) selama jam siang hari kerja. Anda harus mengharapkan bahwa aplikasi ini akan mencapai throughput yang sangat terbatas selama waktu ini. Namun, selama jam malam dan akhir pekan untuk wilayah ini, Layanan akan siap untuk memproses volume permintaan yang jauh lebih tinggi dari aplikasi latar belakang.

**Masalah DLP dengan nomor paspor AS/Inggris**

Apakah Anda mengalami masalah dengan **pencegahan kehilangan data (DLP)** yang tidak bekerja untuk konten yang berisi **nomor paspor AS/Inggris** saat menggunakan jenis informasi sensitif DLP di O365? Jika demikian, pastikan konten Anda berisi informasi yang diperlukan untuk apa kebijakan DLP Cari ketika dievaluasi.
  
Misalnya, untuk kebijakan **nomor paspor AS/Inggris** yang dikonfigurasi dengan tingkat kepercayaan 75%, berikut dievaluasi dan harus terdeteksi untuk aturan untuk memicu
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Sembilan digit

- **[Pola:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Sembilan digit berturut-turut

- **[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Tidak, tidak ada checksum

- **[Definisi:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Sebuah kebijakan DLP adalah 75% yakin bahwa hal itu terdeteksi jenis informasi sensitif jika, dalam kedekatan 300 karakter:

  - Fungsi Func_usa_uk_passport menemukan konten yang sesuai dengan pola.

  - Kata kunci dari Keyword_passport ditemukan.

    Sebagai contoh, contoh berikut akan memicu untuk kebijakan **nomor paspor AS/Inggris** : nomor paspor AS 123456789

Untuk informasi lebih lanjut tentang apa yang diperlukan untuk nomor paspor AS/Inggris yang akan terdeteksi untuk konten Anda, lihat bagian berikut dalam artikel ini: [apa jenis informasi sensitif mencari US/Inggris nomor paspor](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Menggunakan jenis informasi sensitif internal yang berbeda, lihat artikel berikut untuk informasi tentang apa yang diperlukan untuk jenis lain: [apa jenis informasi sensitif](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for) mencari
  