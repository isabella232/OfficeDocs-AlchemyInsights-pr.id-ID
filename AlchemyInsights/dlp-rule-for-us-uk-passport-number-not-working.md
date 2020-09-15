---
title: Aturan DLP untuk nomor paspor AS/Inggris tidak berfungsi
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
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679227"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Masalah dengan DLP-nomor paspor AS/Inggris

**Penting**: Selama masa-masa yang berat ini, kami mengambil langkah untuk memastikan bahwa SharePoint Online dan layanan OneDrive tetap memiliki ketersediaan yang tinggi. Silakan kunjungi [Penyesuaian Fitur Sementara SharePoint Online](https://aka.ms/ODSPAdjustments) untuk informasi selengkapnya.

**Masalah DLP dengan nomor paspor AS/Inggris**

Apakah Anda mengalami masalah dengan **pencegahan kehilangan data (DLP)** tidak berfungsi untuk konten yang berisi **nomor paspor AS/Inggris** saat menggunakan tipe informasi sensitif DLP di O365? Jika demikian, pastikan konten Anda berisi informasi yang diperlukan tentang apa yang dicari kebijakan DLP saat dievaluasi.
  
Misalnya, untuk kebijakan **nomor paspor AS/Inggris** yang dikonfigurasikan dengan tingkat kepercayaan 75%, hal berikut dievaluasi dan harus dideteksi agar aturan dapat dipicu
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Sembilan digit

- **[Pola:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Sembilan digit berurutan

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Tidak, tidak ada checksum

- **[Definisi:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Kebijakan DLP adalah 75% yakin bahwa kebijakan ini mendeteksi tipe informasi sensitif ini jika, dalam kedekatan karakter 300:

  - Fungsi Func_usa_uk_passport menemukan konten yang cocok dengan pola.

  - Kata kunci dari Keyword_passport ditemukan.

    Misalnya, contoh berikut ini akan memicu kebijakan **nomor paspor AS/Inggris** : nomor paspor AS 123456789

Untuk informasi selengkapnya tentang apa yang diperlukan untuk nomor paspor AS/Inggris yang akan terdeteksi untuk konten Anda, lihat bagian berikut ini di artikel ini: [apa tipe informasi sensitif Cari nomor paspor AS/UK](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Menggunakan tipe informasi sensitif bawaan yang berbeda, lihat artikel berikut ini untuk informasi tentang apa yang diperlukan untuk tipe lainnya: [apa yang dicari tipe informasi sensitif](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  