---
title: DLP tidak bekerja seperti yang diharapkan
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 102c8025571f840cf64091d75295acec50661df2
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530287"
---
# <a name="dlp-not-working-as-expected"></a>DLP tidak bekerja seperti yang diharapkan

Apakah Anda memiliki masalah dengan **Data Rugi Pencegahan (DLP)** di Office 365 tidak bekerja seperti yang diharapkan? Jika demikian, pastikan bahwa Anda **DLP kebijakan** diatur dengan benar, dan bahwa data Anda berisi apa **kebijakan DLP** adalah mencari ketika itu sedang dievaluasi.
  
 **Menyiapkan DLP**
  
DLP kebijakan memungkinkan Anda untuk mengidentifikasi dan melindungi informasi sensitif di organisasi Anda. Untuk setup DLP kebijakan, menggunakan informasi [di sini](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **Apa kebijakan DLP mencari**
  
Ketika menggunakan **jenis built-in informasi sensitif** di pusat kantor 365 keamanan dan kepatuhan, DLP kebijakan mencari pola-pola tertentu dan unsur-unsur ketika mendeteksi jenis sensitif.
  
- **Jenis informasi sensitif built-in**

    Untuk informasi tentang built-in tipe sensitif dan apa kebijakan DLP terlihat ketika mendeteksi jenis sensitif, lihat: [apa jenis informasi sensitif yang mencari](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).

- **Jenis informasi sensitif kustom**

    Jika Anda mencoba untuk menciptakan jenis informasi sensitif kustom, menggunakan artikel berikut untuk informasi tentang cara membuat custom jenis sensitif: [membuat sejenis kustom informasi sensitif](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).

**Menguji DLP kebijakan**

Untuk menguji data Anda dengan tipe built-in atau kustom informasi sensitif, menggunakan **jenis Test** opsi di bawah **klasifikasi** > **jenis sensitif info**. Untuk selengkapnya, lihat [jenis informasi sensitif kustom tes](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).

 **Laporan**
  
- Mendapatkan data sensitif wawasan dengan [laporan DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)

- Lihat rincian spesifik dari acara dengan [Insiden Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).
