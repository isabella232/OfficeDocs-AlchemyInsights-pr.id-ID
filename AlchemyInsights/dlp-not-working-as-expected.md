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
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932625"
---
# <a name="dlp-not-working-as-expected"></a>DLP tidak bekerja seperti yang diharapkan

**Penting**: banyak SharePoint online dan OneDrive pelanggan menjalankan aplikasi penting bisnis terhadap layanan yang berjalan di latar belakang. Ini termasuk migrasi konten, pencegahan kehilangan data (DLP), dan solusi pencadangan. Selama waktu yang belum pernah terjadi sebelumnya, kami mengambil langkah untuk memastikan bahwa SharePoint online dan layanan OneDrive tetap sangat tersedia dan dapat diandalkan untuk pengguna yang bergantung pada layanan lebih dari sebelumnya dalam skenario kerja jarak jauh.

Untuk mendukung tujuan ini, kami telah menerapkan batas pelambatan yang lebih ketat pada aplikasi latar belakang (migrasi, DLP dan solusi cadangan) selama jam siang hari kerja. Anda harus mengharapkan bahwa aplikasi ini akan mencapai throughput yang sangat terbatas selama waktu ini. Namun, selama jam malam dan akhir pekan untuk wilayah ini, Layanan akan siap untuk memproses volume permintaan yang jauh lebih tinggi dari aplikasi latar belakang.

 **Menyiapkan DLP**

Apakah Anda mengalami masalah dengan **pencegahan kehilangan data (DLP)** di Office 365 tidak bekerja seperti yang diharapkan? Jika demikian, pastikan bahwa Anda **DLP kebijakan** diatur dengan benar, dan bahwa data Anda berisi apa **kebijakan DLP** sedang mencari ketika sedang dievaluasi.
  
Kebijakan DLP memungkinkan Anda mengidentifikasi dan melindungi informasi sensitif di organisasi Anda. Untuk setup DLP kebijakan, gunakan informasi [di sini](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **Apa yang dicari oleh kebijakan DLP**
  
Saat menggunakan **jenis informasi sensitif internal** di pusat keamanan dan kepatuhan Office 365, kebijakan DLP mencari pola dan elemen tertentu saat mendeteksi jenis sensitif ini.
  
- **Jenis informasi sensitif internal**

    Untuk informasi tentang jenis sensitif internal dan apa yang dicari oleh kebijakan DLP saat mendeteksi jenis sensitif, lihat: [apa jenis informasi sensitif Cari](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).

- **Jenis informasi sensitif khusus**

    Jika Anda mencoba untuk membuat jenis informasi sensitif kustom, gunakan artikel berikut ini untuk informasi tentang cara membuat jenis sensitif kustom: [membuat jenis informasi sensitif kustom](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).

**Menguji kebijakan DLP**

Untuk menguji data Anda dengan jenis informasi sensitif internal atau kustom, gunakan opsi **jenis uji** di bawah **klasifikasi** > **jenis Info sensitif**. Untuk informasi selengkapnya, lihat [menguji jenis informasi sensitif kustom](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).

 **Laporan**
  
- Dapatkan wawasan data sensitif dengan [laporan DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)

- Lihat detail spesifik acara dengan [laporan insiden](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).
