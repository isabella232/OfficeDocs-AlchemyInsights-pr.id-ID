---
title: Aturan DLP untuk SSN tidak berfungsi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 35859bce89ef1ae9b6a9e706fc316b0ee6cd27d1
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507373"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Masalah DLP dengan nomor jaminan sosial

**Penting**: Selama masa-masa yang berat ini, kami mengambil langkah untuk memastikan bahwa SharePoint Online dan layanan OneDrive tetap memiliki ketersediaan yang tinggi. Silakan kunjungi [Penyesuaian Fitur Sementara SharePoint Online](https://aka.ms/ODSPAdjustments) untuk informasi selengkapnya.

**Masalah DLP dengan SSNs**

Apakah Anda mengalami masalah dengan **pencegahan kehilangan data (DLP)** tidak bekerja untuk konten yang berisi **nomor jaminan sosial (SSN)** saat menggunakan jenis informasi sensitif di Microsoft 365? Jika demikian, pastikan konten Anda berisi informasi yang diperlukan untuk apa kebijakan DLP Cari. 
  
Misalnya, untuk kebijakan SSN yang dikonfigurasi dengan tingkat kepercayaan 85%, berikut dievaluasi dan harus terdeteksi untuk aturan untuk memicu:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 digit, yang mungkin dalam pola diformat atau tidak diformat

- **[Pola:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Empat fungsi mencari SSNs dalam empat pola yang berbeda:

  - Func_ssn menemukan SSNs dengan pra-2011 format yang kuat yang diformat dengan tanda hubung atau spasi (DDD-DD-DDDD atau DDD DD DDDD)

  - Func_unformatted_ssn menemukan SSNs dengan pra-2011 format yang kuat yang telah diformat sebagai sembilan digit berturut-turut (ddddddddd)

  - Func_randomized_formatted_ssn menemukan Post-2011 SSNs yang diformat dengan tanda hubung atau spasi (DDD-DD-DDDD atau DDD DD DDDD)

  - Func_randomized_unformatted_ssn menemukan Post-2011 SSNs yang terformat sebagai sembilan digit berturut-turut (ddddddddd)

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Tidak, tidak ada checksum

- **[Definisi:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Sebuah kebijakan DLP adalah 85% yakin bahwa hal itu terdeteksi jenis informasi sensitif jika, dalam kedekatan 300 karakter:

  - [Fungsi Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) menemukan konten yang sesuai dengan pola.

  - Kata kunci dari [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) ditemukan. Contoh kata kunci meliputi: *jaminan sosial, jaminan sosial #, SOC SEC, SSN* . Sebagai contoh, contoh berikut akan memicu kebijakan DLP SSN: **SSN: 489-36-8350**
  
Untuk informasi lebih lanjut tentang apa yang diperlukan untuk SSNs untuk terdeteksi untuk konten Anda, lihat bagian berikut dalam artikel ini: [apa jenis informasi sensitif mencari SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Menggunakan jenis informasi sensitif internal yang berbeda, lihat artikel berikut untuk informasi tentang apa yang diperlukan untuk jenis lain: [apa jenis informasi sensitif](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) mencari
  