---
title: Aturan DLP untuk Nomor Rekening Bank AS tidak berfungsi
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: d19b2dcc29e23fab522159945496165338a117a47bfcfcadf0b93e4e5f14464f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005021"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>Masalah DLP dengan nomor rekening bank AS

**Penting**: Selama masa-masa yang berat ini, kami mengambil langkah untuk memastikan bahwa SharePoint Online dan layanan OneDrive tetap memiliki ketersediaan yang tinggi. Silakan kunjungi [Penyesuaian Fitur Sementara SharePoint Online](https://aka.ms/ODSPAdjustments) untuk informasi selengkapnya.

**Masalah DLP dengan nomor rekening bank AS**

Apakah Anda mengalami masalah dengan **Pencegahan Kehilangan Data (DLP, Data Loss Prevention)** tidak berfungsi untuk konten yang berisi Nomor Rekening **Bank** AS saat menggunakan tipe informasi sensitif DLP di O365? Jika demikian, pastikan konten Anda berisi informasi yang diperlukan untuk apa yang dicari kebijakan DLP saat dievaluasi.
  
Misalnya, untuk kebijakan Nomor Rekening **Bank** AS yang dikonfigurasi dengan tingkat kepercayaan 85%, hal berikut ini dievaluasi dan harus dideteksi agar aturan dapat memicu:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 digit

- **[Pola:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 digit berurutan.

- **[Jumlah Cek:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Tidak, tidak ada Checksum

- **[Definisi:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Kebijakan DLP adalah 75% yakin bahwa DLP mendeteksi tipe informasi sensitif ini jika, dalam kedekatan 300 karakter:

  - Ekspresi reguler Regex_usa_bank_account_number menemukan konten yang cocok dengan pola

  - Kata kunci dari Keyword_usa_Bank_Account ditemukan.

    Misalnya, contoh berikut ini akan memicu kebijakan Nomor **Rekening Bank** AS: Memeriksa Rekening 78344011

Untuk informasi selengkapnya tentang hal-hal yang diperlukan agar Nomor Rekening **Bank** AS terdeteksi bagi konten Anda, lihat bagian berikut dalam artikel ini: Yang cari Nomor Rekening [Bank AS](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Menggunakan tipe informasi bawaan yang berbeda, lihat artikel berikut untuk informasi tentang apa yang diperlukan untuk tipe lain: Apa yang mencari [Tipe Informasi Sensitif](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  