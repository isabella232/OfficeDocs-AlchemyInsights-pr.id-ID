---
title: Aturan DLP untuk SSN tidak berfungsi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679372"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Masalah DLP dengan nomor jaminan sosial

**Penting**: Selama masa-masa yang berat ini, kami mengambil langkah untuk memastikan bahwa SharePoint Online dan layanan OneDrive tetap memiliki ketersediaan yang tinggi. Silakan kunjungi [Penyesuaian Fitur Sementara SharePoint Online](https://aka.ms/ODSPAdjustments) untuk informasi selengkapnya.

**Masalah DLP dengan SSNs**

Apakah Anda mengalami masalah dengan **pencegahan kehilangan data (DLP)** tidak berfungsi untuk konten yang berisi **nomor jaminan sosial (SSN)** saat menggunakan tipe informasi sensitif di Microsoft 365? Jika demikian, pastikan konten Anda berisi informasi yang diperlukan untuk apa yang dicari kebijakan DLP. 
  
Misalnya, untuk kebijakan SSN yang dikonfigurasi dengan tingkat kepercayaan 85%, berikut ini dievaluasi dan harus dideteksi agar aturan dipicu:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 digit, yang mungkin dalam pola yang diformat atau tidak diformat

- **[Pola:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Empat fungsi mencari SSNs dalam empat pola yang berbeda:

  - Func_ssn menemukan SSNs dengan pemformatan pra-2011 kuat yang diformat dengan garis putus-putus atau spasi (DDD-DD-DDDD atau DDD DD DDDD)

  - Func_unformatted_ssn menemukan SSNs dengan pemformatan pra-2011 yang kuat yang tidak diformat sebagai sembilan digit berturut-turut (ddddddddd)

  - Func_randomized_formatted_ssn menemukan SSNs Post-2011 yang diformat dengan garis putus-putus atau spasi (DDD-DD-DDDD atau DDD DD DDDD)

  - Func_randomized_unformatted_ssn menemukan SSNs Post-2011 yang tidak diformat sebagai sembilan digit berturut-turut (ddddddddd)

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Tidak, tidak ada checksum

- **[Definisi:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Kebijakan DLP adalah 85% yakin bahwa kebijakan ini mendeteksi tipe informasi sensitif ini jika, dalam kedekatan karakter 300:

  - [Fungsi Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) menemukan konten yang cocok dengan pola.

  - Kata kunci dari [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) ditemukan. Contoh kata kunci meliputi: Jamsostek  *, Jamsostek #, SOC SEC, SSN*  . Misalnya, contoh berikut ini akan memicu kebijakan SSN DLP: **SSN: 489-36-8350**
  
Untuk informasi lebih lanjut tentang apa yang diperlukan untuk SSNs yang akan terdeteksi untuk konten Anda, lihat bagian berikut ini di artikel ini: [apa tipe informasi sensitif Cari SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Menggunakan tipe informasi sensitif bawaan yang berbeda, lihat artikel berikut ini untuk informasi tentang apa yang diperlukan untuk tipe lainnya: [apa yang dicari tipe informasi sensitif](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  