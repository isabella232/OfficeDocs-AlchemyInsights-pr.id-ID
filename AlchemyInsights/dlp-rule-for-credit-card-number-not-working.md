---
title: Aturan DLP untuk Nomor Kartu Kredit tidak berfungsi
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
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: bd4f200233d5571fc7b01576038e7b3951a07716a7d5948005418d2896291ee5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005093"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Masalah DLP dengan nomor kartu kredit

**Penting**: Selama masa-masa yang berat ini, kami mengambil langkah untuk memastikan bahwa SharePoint Online dan layanan OneDrive tetap memiliki ketersediaan yang tinggi. Silakan kunjungi [Penyesuaian Fitur Sementara SharePoint Online](https://aka.ms/ODSPAdjustments) untuk informasi selengkapnya.

**Masalah DLP dengan nomor kartu kredit**

Apakah Anda mengalami masalah dengan **Pencegahan Kehilangan Data (DLP, Data Loss Prevention)** tidak berfungsi untuk konten yang berisi Nomor Kartu Kredit saat menggunakan tipe informasi sensitif DLP di O365?  Jika demikian, pastikan konten Anda berisi informasi yang diperlukan untuk memicu kebijakan DLP saat dievaluasi. Misalnya, untuk **kebijakan** Kartu Kredit yang dikonfigurasi dengan tingkat kepercayaan 85%, hal berikut ini dievaluasi dan harus dideteksi agar aturan dapat memicu:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 digit yang bisa diformat atau tidak diformat (dddddddddddddd) dan harus lolos uji Luhn.

- **[Pola:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Pola yang sangat kompleks dan kokoh yang mendeteksi kartu dari semua merek utama di seluruh dunia, termasuk Visa, MasterCard, Discover Card, JCB, American Express, kartu hadiah, dan kartu diner.

- **[Jumlah Cek:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Ya, checksum Luhn

- **[Definisi:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Kebijakan DLP adalah 85% yakin bahwa DLP mendeteksi tipe informasi sensitif ini jika, dalam kedekatan 300 karakter:

  - Fungsi yang Func_credit_card menemukan konten yang cocok dengan pola.

  - Salah satu hal berikut ini benar:

  - Kata kunci dari Keyword_cc_verification ditemukan.

  - Kata kunci Keyword_cc_name ditemukan

  - Fungsi Func_expiration_date menemukan tanggal dalam format tanggal yang tepat.

  - Jumlah cek masuk

    Misalnya, sampel berikut akan memicu untuk Kebijakan Nomor Kartu Kredit DLP:

  - Visa: 4485 3647 3952 7352
  
  - Kedaluwarsa: 2/2009

Untuk informasi selengkapnya tentang apa  yang diperlukan agar Nomor Kartu Kredit dapat dideteksi untuk konten Anda, lihat bagian berikut dalam artikel ini: Apa itu Tipe Informasi Sensitif [untuk Kartu Kredit#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Menggunakan tipe informasi bawaan yang berbeda, lihat artikel berikut untuk informasi tentang apa yang diperlukan untuk tipe lain: Apa yang mencari [Tipe Informasi Sensitif](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  