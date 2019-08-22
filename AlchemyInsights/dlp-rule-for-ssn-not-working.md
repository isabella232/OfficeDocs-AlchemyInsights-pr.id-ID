---
title: DLP aturan untuk SSN tidak bekerja
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
ms.openlocfilehash: 757136c39700f12f40f839b29277a59b0e436f03
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529860"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP masalah dengan nomor jaminan sosial

Apakah Anda memiliki masalah dengan **Data Rugi Pencegahan (DLP)** tidak bekerja untuk konten yang berisi **Nomor jaminan sosial (SSN)** ketika menggunakan jenis informasi sensitif di Office 365? Jika demikian, pastikan konten Anda berisi informasi yang dibutuhkan untuk apa kebijakan DLP Cari. 
  
Misalnya, untuk kebijakan SSN dikonfigurasi dengan tingkat keyakinan 85%, berikut dievaluasi dan harus terdeteksi untuk aturan untuk memicu:
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digit, yang mungkin dalam pola diformat atau tidak diformat

- **[Pola:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Empat fungsi Cari SSNs dalam empat pola yang berbeda:

  - Func_ssn menemukan SSNs dengan pra-2011 kuat format yang diformat dengan tanda hubung atau ruang (ddd-dd-dddd OR ddd dd dddd)

  - Func_unformatted_ssn menemukan SSNs dengan pra-2011 kuat format yang tidak diformat sebagai sembilan angka berturut-turut (ddddddddd)

  - Func_randomized_formatted_ssn menemukan posting-2011 SSNs yang diformat dengan tanda hubung atau ruang (ddd-dd-dddd OR ddd dd dddd)

  - Func_randomized_unformatted_ssn menemukan posting-2011 SSNs yang tidak diformat sebagai sembilan angka berturut-turut (ddddddddd)

- **[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Tidak, adalah tidak terdapat Checksum

- **[Definisi:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Kebijakan DLP adalah 85% yakin bahwa ia telah mendeteksi jenis informasi sensitif jika, dalam jarak 300 karakter:

  - [Fungsi Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) menemukan konten yang cocok dengan pola.

  - Kata kunci dari [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) ditemukan. Contoh kata kunci mencakup: *jaminan sosial, Jamsostek #, Soc Sec, SSN* . Misalnya, contoh berikut akan memicu untuk kebijakan DLP SSN: **SSN: 489-36-8350**
  
Untuk informasi lebih lanjut tentang apa yang diperlukan untuk SSNs untuk dideteksi untuk konten Anda, lihat bagian berikut dalam artikel ini: [Apa the sensitif informasi jenis mencari SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Menggunakan jenis informasi sensitif built-in yang berbeda, lihat artikel berikut untuk informasi apa saja diperlukan untuk jenis lainnya: [apa the sensitif informasi jenis mencari](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  