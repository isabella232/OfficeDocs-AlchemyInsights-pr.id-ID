---
title: SharePoint migrasi pelambatan dengan galat 503
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 7e12c74d33e3cee7c626ad899a4e7f2f0a409bca
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931661"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a>SharePoint migrasi pelambatan dengan galat 503

**Penting**: banyak SharePoint online dan OneDrive pelanggan menjalankan aplikasi penting bisnis terhadap layanan yang berjalan di latar belakang. Ini termasuk migrasi konten, pencegahan kehilangan data (DLP), dan solusi pencadangan. Selama waktu yang belum pernah terjadi sebelumnya, kami mengambil langkah untuk memastikan bahwa SharePoint online dan layanan OneDrive tetap sangat tersedia dan dapat diandalkan untuk pengguna yang bergantung pada layanan lebih dari sebelumnya dalam skenario kerja jarak jauh.

Untuk mendukung tujuan ini, kami telah menerapkan batas pelambatan yang lebih ketat pada aplikasi latar belakang (migrasi, DLP dan solusi cadangan) selama jam siang hari kerja. Anda harus mengharapkan bahwa aplikasi ini akan mencapai throughput yang sangat terbatas selama waktu ini. Namun, selama jam malam dan akhir pekan untuk wilayah ini, Layanan akan siap untuk memproses volume permintaan yang jauh lebih tinggi dari aplikasi latar belakang.

**503 galat saat migrasi ke SharePoint online**

Tampaknya Anda bermigrasi ke SharePoint online dan menerima 503 kesalahan. Silakan ikuti langkah di bawah ini sehingga kami dapat membantu Anda sesegera mungkin. 

1. Klik **Hubungi dukungan**, dan kemudian **permintaan layanan baru**.
2. Untuk judul dan deskripsi, ketik **migrasi throttling SharePoint dengan 503**.
3. Setelah tiket diserahkan, silakan update dengan informasi berikut:
    - Berapa banyak sisa migrasi (misalnya, berapa banyak TBs?).
    - Tanggal mulai dan akhir migrasi.
    - Jelaskan di mana Anda memigrasi konten, seperti SharePoint Server, kotak, GDrive, berbagi file, dsb.
    - Perkirakan jumlah kesalahan pelambatan (misalnya, x throttle per jam?) dan Kapan pelambatan terjadi.
    - Alat migrasi yang Anda gunakan (misalnya, SPMT atau ShareGate).


