---
title: DLP aturan untuk nomor kartu kredit tidak bekerja
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
ms.openlocfilehash: 5d3bdb3b074c485a2b19e934724ba6e74c84deae
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389580"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP masalah dengan nomor kartu kredit

Apakah Anda memiliki masalah dengan **Data Rugi Pencegahan (DLP)** tidak bekerja untuk konten yang berisi **Nomor kartu kredit** ketika menggunakan jenis informasi sensitif DLP di O365? Jika demikian, pastikan konten Anda berisi informasi yang diperlukan untuk memicu kebijakan DLP ketika itu dievaluasi. Misalnya, **kartu kredit kebijakan** dikonfigurasi dengan tingkat keyakinan 85%, berikut dievaluasi dan harus terdeteksi untuk aturan untuk memicu:
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digit yang dapat diformat atau tidak diformat (dddddddddddddddd) dan harus lulus tes Luhn.

- **[Pola:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Sangat kompleks dan kuat pola yang mendeteksi kartu dari semua merek utama di seluruh dunia, termasuk Visa, MasterCard, Discover Card, JCB, kartu American Express, kartu hadiah, dan restoran.

- **[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Ya, Luhn checksum

- **[Definisi:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Kebijakan DLP adalah 85% yakin bahwa ia telah mendeteksi jenis informasi sensitif jika, dalam jarak 300 karakter:

  - Fungsi Func_credit_card menemukan konten yang cocok dengan pola.

  - Salah satu dari berikut ini benar:

  - Kata kunci dari Keyword_cc_verification ditemukan.

  - Kata kunci dari Keyword_cc_name ditemukan

  - Fungsi Func_expiration_date menemukan tanggal dalam format tanggal yang tepat.

  - Checksum melewati

    Misalnya, contoh berikut akan memicu DLP kartu kredit nomor kebijakan:

  - Visa: 4485 3647 3952 7352
  
  - Berakhir: 2/2009

Untuk informasi lebih lanjut tentang apa saja diperlukan untuk **Nomor kartu kredit** untuk terdeteksi untuk konten Anda, lihat bagian berikut dalam artikel ini: [Apa the sensitif informasi jenis mencari kartu kredit #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Menggunakan jenis informasi sensitif built-in yang berbeda, lihat artikel berikut untuk informasi apa saja diperlukan untuk jenis lainnya: [apa the sensitif informasi jenis mencari](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  