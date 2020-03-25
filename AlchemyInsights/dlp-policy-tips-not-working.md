---
title: Tips DLP kebijakan tidak bekerja
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932589"
---
# <a name="dlp-policy-tip-issues"></a>Masalah DLP kebijakan Tips

**Penting**: banyak SharePoint online dan OneDrive pelanggan menjalankan aplikasi penting bisnis terhadap layanan yang berjalan di latar belakang. Ini termasuk migrasi konten, pencegahan kehilangan data (DLP), dan solusi pencadangan. Selama waktu yang belum pernah terjadi sebelumnya, kami mengambil langkah untuk memastikan bahwa SharePoint online dan layanan OneDrive tetap sangat tersedia dan dapat diandalkan untuk pengguna yang bergantung pada layanan lebih dari sebelumnya dalam skenario kerja jarak jauh.

Untuk mendukung tujuan ini, kami telah menerapkan batas pelambatan yang lebih ketat pada aplikasi latar belakang (migrasi, DLP dan solusi cadangan) selama jam siang hari kerja. Anda harus mengharapkan bahwa aplikasi ini akan mencapai throughput yang sangat terbatas selama waktu ini. Namun, selama jam malam dan akhir pekan untuk wilayah ini, Layanan akan siap untuk memproses volume permintaan yang jauh lebih tinggi dari aplikasi latar belakang.

**Tips kebijakan DLP**

Saat menggunakan **kebijakan DLP**, pengguna dapat diberitahu tentang pelanggaran kebijakan dengan **Tips kebijakan**. Admin dapat mengkonfigurasi kebijakan Tips untuk menampilkan saat pengujian kebijakan DLP mereka atau ketika kebijakan dalam mode penegakan penuh.
  
Untuk mengkonfigurasi Tips kebijakan DLP kebijakan di pusat keamanan dan kepatuhan dalam mode penegakan penuh, lakukan hal berikut:
  
- Pastikan kiat kebijakan telah **diaktifkan** pada aturan DLP dengan menggunakan langkah [di sini](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).

- Pastikan **konten Anda sesuai** dengan apa yang **diperlukan** untuk memicu aturan yang diuraikan dalam artikel ini di [sini](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).

- Tips kebijakan ditampilkan di OWA dan Outlook. Namun, saat menggunakan **Outlook 2013 atau yang lebih baru**, Tips kebijakan hanya ditampilkan di bawah kondisi tertentu. Kondisi ini tercantum di sini: [kondisi yang didukung untuk Outlook 2013 atau yang lebih baru untuk menampilkan Tips kebijakan](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)

Untuk informasi tambahan tentang Tips DLP kebijakan, lihat: [Tampilkan Tips kebijakan DLP kebijakan](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)
  