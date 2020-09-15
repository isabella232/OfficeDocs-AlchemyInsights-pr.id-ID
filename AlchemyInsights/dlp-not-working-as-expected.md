---
title: DLP tidak berfungsi seperti yang diharapkan
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
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0ed893420b5813d5d18639c2c226c12f0306a13f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679696"
---
# <a name="dlp-not-working-as-expected"></a>DLP tidak berfungsi seperti yang diharapkan

**Penting**: Selama masa-masa yang berat ini, kami mengambil langkah untuk memastikan bahwa SharePoint Online dan layanan OneDrive tetap memiliki ketersediaan yang tinggi. Silakan kunjungi [Penyesuaian Fitur Sementara SharePoint Online](https://aka.ms/ODSPAdjustments) untuk informasi selengkapnya.

 **Menyiapkan DLP**

Apakah Anda mengalami masalah dengan **pencegahan kehilangan data (DLP)** di Office 365 tidak berfungsi seperti yang diharapkan? Jika demikian, pastikan bahwa **kebijakan DLP** Anda disetel dengan benar, dan bahwa data Anda berisi apa yang dicari **kebijakan DLP** saat dievaluasi.
  
Kebijakan DLP memungkinkan Anda mengidentifikasi dan melindungi informasi sensitif di organisasi Anda. Untuk menyetel kebijakan DLP, gunakan informasi [di sini](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **Apa yang dicari kebijakan DLP**
  
Saat menggunakan **tipe informasi sensitif bawaan** di pusat keamanan dan kepatuhan, kebijakan DLP mencari pola dan elemen tertentu saat mendeteksi tipe sensitif ini.
  
- **Tipe informasi sensitif bawaan**

    Untuk informasi tentang tipe sensitif bawaan dan apa yang dicari kebijakan DLP saat mendeteksi tipe sensitif, lihat: [seperti apa tipe informasi sensitif tersebut](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

- **Tipe informasi sensitif kustom**

    Jika Anda mencoba membuat tipe informasi sensitif kustom, gunakan artikel berikut ini untuk informasi tentang cara membuat tipe sensitif kustom: [membuat tipe informasi sensitif kustom](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).

**Menguji kebijakan DLP**

Untuk menguji data Anda dengan tipe informasi sensitif bawaan atau kustom, gunakan opsi **tipe uji** di bawah tipe informasi sensitif **klasifikasi**  >  **Sensitive info types**. Untuk informasi selengkapnya, lihat [menguji tipe informasi sensitif kustom](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).

 **Melaporkan**
  
- Dapatkan wawasan data sensitif dengan [laporan DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Lihat detail acara tertentu dengan [laporan insiden](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).
