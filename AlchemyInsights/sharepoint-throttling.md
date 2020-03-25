---
title: Pelambatan SharePoint online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 9af4f09d50992c04a1f3d5a164093049a3ec3517
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931445"
---
# <a name="sharepoint-online-throttling"></a>Pelambatan SharePoint online

**Penting**: banyak SharePoint online dan OneDrive pelanggan menjalankan aplikasi penting bisnis terhadap layanan yang berjalan di latar belakang. Ini termasuk migrasi konten, pencegahan kehilangan data (DLP), dan solusi pencadangan. Selama waktu yang belum pernah terjadi sebelumnya, kami mengambil langkah untuk memastikan bahwa SharePoint online dan layanan OneDrive tetap sangat tersedia dan dapat diandalkan untuk pengguna yang bergantung pada layanan lebih dari sebelumnya dalam skenario kerja jarak jauh.

Untuk mendukung tujuan ini, kami telah menerapkan batas pelambatan yang lebih ketat pada aplikasi latar belakang (migrasi, DLP dan solusi cadangan) selama jam siang hari kerja. Anda harus mengharapkan bahwa aplikasi ini akan mencapai throughput yang sangat terbatas selama waktu ini. Namun, selama jam malam dan akhir pekan untuk wilayah ini, Layanan akan siap untuk memproses volume permintaan yang jauh lebih tinggi dari aplikasi latar belakang.

**Pelambatan SharePoint online**

SharePoint Online menggunakan pelambatan untuk mempertahankan kinerja optimal dan keandalan Layanan SharePoint online. Pelambatan membatasi jumlah tindakan pengguna atau panggilan bersamaan (dengan skrip atau kode) untuk mencegah penggunaan sumber daya berlebihan. Untuk informasi lebih lanjut, silakan kunjungi link di bawah ini.

- [Hindari mendapatkan mengalami kelambatan atau diblokir di SharePoint online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [Data migrasi dan SPO throttling](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)

- [SharePoint online dan OneDrive kecepatan migrasi](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

 - [Menangani SharePoint online pelambatan menggunakan eksponensial mundur](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)

- [Perencanaan kapasitas dan pengujian beban SharePoint online](https://docs.microsoft.com/office365/enterprise/capacity-planning-and-load-testing-sharepoint-online)

