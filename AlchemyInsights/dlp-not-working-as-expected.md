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
ms.openlocfilehash: e1049f160a9b92040095b6725fa5771218a0956d17f99ea8a6e9cc279e7c73f6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079705"
---
# <a name="dlp-not-working-as-expected"></a>DLP tidak berfungsi seperti yang diharapkan

**Penting**: Selama masa-masa yang berat ini, kami mengambil langkah untuk memastikan bahwa SharePoint Online dan layanan OneDrive tetap memiliki ketersediaan yang tinggi. Silakan kunjungi [Penyesuaian Fitur Sementara SharePoint Online](https://aka.ms/ODSPAdjustments) untuk informasi selengkapnya.

 **Menyiapkan DLP**

Apakah Anda mengalami masalah dengan **Pencegahan Kehilangan Data (DLP, Data Loss Prevention)** Office 365 tidak berfungsi seperti yang diharapkan? If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.
  
Kebijakan DLP memungkinkan Anda mengidentifikasi dan melindungi informasi sensitif di organisasi Anda. Untuk menyiapkan kebijakan DLP, gunakan informasi di [sini](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).
  
 **Apa yang terlihat oleh kebijakan DLP**
  
Saat menggunakan **tipe informasi** sensitif bawaan di pusat Keamanan dan Kepatuhan, kebijakan DLP mencari pola dan elemen tertentu saat mendeteksi tipe sensitif ini.
  
- **Tipe Informasi Sensitif Bawaan**

    Untuk informasi tentang tipe Sensitif bawaan dan apa yang terlihat oleh kebijakan DLP saat mendeteksi tipe Sensitif, lihat: Apa tipe informasi [sensitif mencari](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

- **Tipe Informasi Sensitif Kustom**

    Jika Anda mencoba membuat tipe informasi sensitif kustom, gunakan artikel berikut ini untuk informasi tentang cara membuat tipe sensitif kustom: Membuat tipe informasi [sensitif kustom.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)

**Menguji kebijakan DLP**

Untuk menguji data dengan tipe informasi bawaan atau sensitif kustom, gunakan opsi **Tipe uji** di bawah Klasifikasi **Tipe**  >  **informasi sensitif**. Untuk informasi selengkapnya, lihat [Menguji tipe informasi sensitif kustom.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)

 **Laporan**
  
- Dapatkan wawasan data sensitif dengan [Laporan DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Lihat detail spesifik acara dengan [Laporan Insiden.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)
