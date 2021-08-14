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
ms.openlocfilehash: 3f30998fb3bc4c5442e4e1541b87d88ecd7df6eef3a50e719fa5014eb86af39c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004985"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Masalah DLP dengan Nomor Jaminan Sosial

**Penting**: Selama masa-masa yang berat ini, kami mengambil langkah untuk memastikan bahwa SharePoint Online dan layanan OneDrive tetap memiliki ketersediaan yang tinggi. Silakan kunjungi [Penyesuaian Fitur Sementara SharePoint Online](https://aka.ms/ODSPAdjustments) untuk informasi selengkapnya.

**Masalah DLP dengan SSN**

Apakah Anda mengalami masalah dengan Pencegahan **Hilangnya Data (DLP, Data Loss Prevention)** tidak berfungsi untuk konten yang berisi Nomor Jaminan Sosial **(SSN, Social Security Number)** saat menggunakan tipe informasi sensitif dalam Microsoft 365? Jika demikian, pastikan konten Anda berisi informasi yang diperlukan untuk apa yang terlihat kebijakan DLP. 
  
Misalnya, untuk kebijakan SSN yang dikonfigurasi dengan tingkat kepercayaan 85%, hal berikut ini dievaluasi dan harus dideteksi agar aturan memicu:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 digit, yang mungkin berada dalam pola yang diformat atau tidak diformat

- **[Pola:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Empat fungsi mencari SSN dalam empat pola berbeda:

  - Func_ssn menemukan SSN dengan pemformatan kuat pra-2011 yang diformat dengan garis putus-putus atau spasi (ddd-dd-dddd OR ddd dd dd)

  - Func_unformatted_ssn menemukan SSN dengan pemformatan kuat pra-2011 yang tidak diformat sebagai sembilan digit berturut-turut (ddddddddd)

  - Func_randomized_formatted_ssn menemukan SSN pasca-2011 yang diformat dengan garis putus-putus atau spasi (ddd-dd-dddd OR ddd dd dd)

  - Func_randomized_unformatted_ssn menemukan pasca-2011 SSN yang tidak diformat sebagai sembilan digit berturut-turut (ddddddddd)

- **[Jumlah Cek:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Tidak, tidak ada Checksum

- **[Definisi:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Kebijakan DLP adalah 85% yakin bahwa DLP mendeteksi tipe informasi sensitif ini jika, dalam kedekatan 300 karakter:

  - Fungsi [yang Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) menemukan konten yang cocok dengan pola tersebut.

  - Kata kunci dari [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) ditemukan. Contoh kata kunci meliputi: Jaminan  *Sosial, Jaminan Sosial#, Soc Sec , SSN*  . Misalnya, sampel berikut akan memicu untuk kebijakan SSN DLP: **SSN: 489-36-8350**
  
Untuk informasi selengkapnya tentang apa yang diperlukan agar SSN dideteksi untuk konten Anda, lihat bagian berikut di artikel ini: Apa yang diperlukan tipe Informasi Sensitif untuk [SSN](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Menggunakan tipe informasi bawaan yang berbeda, lihat artikel berikut untuk informasi tentang apa yang diperlukan untuk tipe lain: Apa yang mencari [Tipe Informasi Sensitif](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  