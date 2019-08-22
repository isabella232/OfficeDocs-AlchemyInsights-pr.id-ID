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
ms.openlocfilehash: 8886d7a6fad49e942e17f6a2f3c98542f87aae0b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36495754"
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