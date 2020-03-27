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
ms.openlocfilehash: 4ec0df9d4954a8c65f0c34188d285dd8cf44a4f2
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977309"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Masalah DLP dengan nomor jaminan sosial

**Penting**: selama waktu yang belum pernah terjadi sebelumnya, kami mengambil langkah untuk memastikan bahwa Layanan SharePoint online dan OneDrive tetap sangat tersedia-silakan kunjungi [penyesuaian fitur sementara SharePoint online](https://aka.ms/ODSPAdjustments) untuk informasi lebih lanjut.

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
  