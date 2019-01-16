---
title: DLP aturan untuk US / nomor paspor Inggris tidak bekerja
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 716d1030d93ce006c36d7925fb132e974ae8feb4
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/15/2019
ms.locfileid: "28295597"
---
Apakah Anda mengalami masalah dengan **Data Rugi Pencegahan (DLP)** tidak bekerja karena mengandung konten **U.S. / nomor paspor Inggris** ketika menggunakan jenis informasi sensitif DLP di O365? Jika demikian, pastikan konten Anda berisi informasi yang dibutuhkan untuk apa kebijakan DLP dicari ketika itu dievaluasi. 
  
Misalnya, untuk **U.S. / nomor paspor Inggris** kebijakan dikonfigurasi dengan tingkat keyakinan 75%, berikut dievaluasi dan harus terdeteksi untuk aturan untuk memicu 
  
- **[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Sembilan angka 
    
- **[Pola:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Sembilan angka berturut-turut 
    
- **[Checksum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Tidak, adalah tidak terdapat Checksum 
    
- **[Definisi:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Kebijakan DLP adalah 75% yakin bahwa ia telah mendeteksi jenis informasi sensitif jika, dalam jarak 300 karakter: 
    
  - Fungsi Func_usa_uk_passport menemukan konten yang cocok dengan pola.
    
  - Kata kunci dari Keyword_passport ditemukan.
    
    Misalnya, contoh berikut akan memicu untuk **U.S. / nomor paspor Inggris** kebijakan: nomor paspor AS 123456789 
    
Untuk informasi lebih lanjut tentang apa saja diperlukan untuk US / nomor paspor Inggris untuk terdeteksi untuk konten Anda, lihat bagian berikut dalam artikel ini: [apa the sensitif informasi jenis tampilan untuk US / nomor paspor Inggris](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Menggunakan jenis informasi sensitif built-in yang berbeda, lihat artikel berikut untuk informasi apa saja diperlukan untuk jenis lainnya: [apa the sensitif informasi jenis mencari](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

