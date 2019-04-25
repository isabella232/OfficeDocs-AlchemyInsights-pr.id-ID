---
title: DLP aturan untuk kami nomor rekening Bank tidak bekerja
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 9ebfa6bc09cef9ab7c30bddb4fcb8b6be3ab55a5
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404272"
---
Apakah Anda memiliki masalah dengan **Data Rugi Pencegahan (DLP)** tidak bekerja untuk konten yang berisi **Nomor rekening Bank US** ketika menggunakan jenis informasi sensitif DLP di O365? Jika demikian, pastikan konten Anda berisi informasi yang dibutuhkan untuk apa kebijakan DLP dicari ketika itu dievaluasi. 
  
Misalnya, **Nomor rekening Bank US** kebijakan dikonfigurasi dengan tingkat keyakinan 85%, berikut dievaluasi dan harus terdeteksi untuk aturan untuk memicu: 
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digit 
    
- **[Pola:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 berturut-turut digit. 
    
- **[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Tidak, adalah tidak terdapat Checksum 
    
- **[Definisi:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Kebijakan DLP adalah 75% yakin bahwa ia telah mendeteksi jenis informasi sensitif jika, dalam jarak 300 karakter: 
    
  - Ekspresi reguler Regex_usa_bank_account_number menemukan konten yang cocok dengan pola
    
  - Kata kunci dari Keyword_usa_Bank_Account ditemukan.
    
    Misalnya, contoh berikut akan memicu untuk kebijakan **Nomor rekening Bank US** : rekening 78344011 
    
Untuk informasi lebih lanjut tentang apa saja diperlukan untuk **Nomor rekening Bank US** untuk terdeteksi untuk konten Anda, lihat bagian berikut dalam artikel ini: [Apa the sensitif informasi jenis mencari nomor rekening Bank US](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
Menggunakan jenis informasi sensitif built-in yang berbeda, lihat artikel berikut untuk informasi apa saja diperlukan untuk jenis lainnya: [apa the sensitif informasi jenis mencari](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

