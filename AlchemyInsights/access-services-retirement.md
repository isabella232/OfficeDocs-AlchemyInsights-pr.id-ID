---
title: Akses layanan pensiun
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 5f171050479f34077f3dc155bec40437f86b84c0
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/28/2019
ms.locfileid: "35359352"
---
# <a name="access-services-retirement"></a>Akses layanan pensiun

Seperti yang kita awalnya diumumkan di MC97576, pada Maret 2017, dan terus berkomunikasi selama setahun layanan akses yang sedang dihentikan dari Office 365. Tahap berikutnya dalam proses ini akan penghapusan akses Web database yang menggunakan daftar SharePoint sebagai penyimpanan data yang mendasari mereka.

**Bagaimana ini mempengaruhi saya?**

Mulai Juni 2019, kami akan berhenti penciptaan baru akses database dalam SharePoint Online dan menutup layanan dan aplikasi sisa 2020 April.

**Apa yang harus saya lakukan untuk mempersiapkan untuk perubahan ini?**

Kami mendorong Anda untuk membuat rencana transisi untuk organisasi Anda akses web database. Admin dapat menggunakan [scanner aplikasi SharePoint akses](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) untuk memperoleh inventarisasi akses aplikasi yang menggunakan situs.

Ada beberapa cara untuk memigrasi data database Access web:

- Mengimpor ke database akses lokal (. ACCDB) atau ke Excel file.
- Kami juga merekomendasikan menjelajahi Microsoft PowerApps sebagai platform alternatif untuk menciptakan solusi bisnis tidak kode untuk web dan perangkat mobile.