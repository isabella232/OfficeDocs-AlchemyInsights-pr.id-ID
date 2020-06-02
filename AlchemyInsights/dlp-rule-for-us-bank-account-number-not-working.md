---
title: Aturan DLP untuk nomor rekening bank AS tidak berfungsi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: b032a7c80e8b387114aeda95c4f6af7e57225517
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507337"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>Masalah DLP dengan nomor rekening bank AS

**Penting**: Selama masa-masa yang berat ini, kami mengambil langkah untuk memastikan bahwa SharePoint Online dan layanan OneDrive tetap memiliki ketersediaan yang tinggi. Silakan kunjungi [Penyesuaian Fitur Sementara SharePoint Online](https://aka.ms/ODSPAdjustments) untuk informasi selengkapnya.

**Masalah DLP dengan nomor rekening bank AS**

Apakah Anda mengalami masalah dengan **pencegahan kehilangan data (DLP)** yang tidak berfungsi untuk konten yang berisi **nomor rekening bank AS** saat menggunakan jenis informasi sensitif DLP di O365? Jika demikian, pastikan konten Anda berisi informasi yang diperlukan untuk apa kebijakan DLP Cari ketika dievaluasi.
  
Misalnya, untuk kebijakan **nomor rekening bank AS** yang dikonfigurasi dengan tingkat kepercayaan 85%, berikut dievaluasi dan harus terdeteksi aturan untuk memicu:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 digit

- **[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 digit berturut-turut.

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Tidak, tidak ada checksum

- **[Definisi:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Sebuah kebijakan DLP adalah 75% yakin bahwa hal itu terdeteksi jenis informasi sensitif jika, dalam kedekatan 300 karakter:

  - Ekspresi reguler Regex_usa_bank_account_number menemukan konten yang sesuai dengan pola

  - Kata kunci dari Keyword_usa_Bank_Account ditemukan.

    Sebagai contoh, contoh berikut akan memicu untuk kebijakan **nomor rekening bank AS** : memeriksa akun 78344011

Untuk informasi lebih lanjut tentang apa yang diperlukan untuk **nomor rekening bank AS** untuk terdeteksi untuk konten Anda, lihat bagian berikut dalam artikel ini: [apa jenis informasi sensitif mencari nomor rekening bank AS](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Menggunakan jenis informasi sensitif internal yang berbeda, lihat artikel berikut untuk informasi tentang apa yang diperlukan untuk jenis lain: [apa jenis informasi sensitif](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) mencari
  