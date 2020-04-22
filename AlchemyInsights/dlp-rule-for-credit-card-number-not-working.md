---
title: Aturan DLP untuk nomor kartu kredit tidak berfungsi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 80ff41b3e746f95278ccbf0df19eebb61f7f9ee0
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704204"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Masalah DLP dengan nomor kartu kredit

**Penting**: Selama masa-masa yang berat ini, kami mengambil langkah untuk memastikan bahwa SharePoint Online dan layanan OneDrive tetap memiliki ketersediaan yang tinggi. Silakan kunjungi [Penyesuaian Fitur Sementara SharePoint Online](https://aka.ms/ODSPAdjustments) untuk informasi selengkapnya.

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
  