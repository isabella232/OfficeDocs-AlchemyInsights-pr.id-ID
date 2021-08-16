---
title: Aturan DLP untuk Nomor Paspor AS/Inggris tidak berfungsi
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 85e3ed7fdc221981de13ab6e2ada8adf2a3a80b40ff163981e047cc4a02a1514
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004949"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Masalah dengan DLP - nomor paspor AS/Inggris

**Penting**: Selama masa-masa yang berat ini, kami mengambil langkah untuk memastikan bahwa SharePoint Online dan layanan OneDrive tetap memiliki ketersediaan yang tinggi. Silakan kunjungi [Penyesuaian Fitur Sementara SharePoint Online](https://aka.ms/ODSPAdjustments) untuk informasi selengkapnya.

**Masalah DLP dengan nomor paspor AS/Inggris**

Apakah Anda mengalami masalah dengan **Pencegahan Hilangnya Data (DLP, Data Loss Prevention)** tidak berfungsi untuk konten yang berisi nomor paspor **AS/UK** saat menggunakan tipe informasi sensitif DLP di O365? Jika demikian, pastikan konten Anda berisi informasi yang diperlukan untuk apa yang dicari kebijakan DLP saat dievaluasi.
  
Misalnya, untuk kebijakan nomor paspor **AS/Inggris** yang dikonfigurasi dengan tingkat kepercayaan 75%, hal berikut ini dievaluasi dan harus dideteksi agar aturan dapat memicu
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Sembilan digit

- **[Pola:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Sembilan digit berurutan

- **[Jumlah Cek:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Tidak, tidak ada Checksum

- **[Definisi:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Kebijakan DLP adalah 75% yakin bahwa DLP mendeteksi tipe informasi sensitif ini jika, dalam kedekatan 300 karakter:

  - Fungsi yang Func_usa_uk_passport menemukan konten yang cocok dengan pola tersebut.

  - Kata kunci dari Keyword_passport ditemukan.

    Misalnya, contoh berikut ini akan memicu kebijakan **nomor paspor AS/Inggris:** Nomor paspor A.S. 123456789

Untuk informasi selengkapnya tentang hal-hal yang diperlukan agar Nomor Paspor AS/Inggris terdeteksi untuk konten Anda, lihat bagian berikut dalam artikel ini: Yang cari Tipe Informasi Sensitif untuk Nomor Paspor [AS/Inggris](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Menggunakan tipe informasi bawaan yang berbeda, lihat artikel berikut untuk informasi tentang apa yang diperlukan untuk tipe lain: Apa yang mencari [Tipe Informasi Sensitif](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  