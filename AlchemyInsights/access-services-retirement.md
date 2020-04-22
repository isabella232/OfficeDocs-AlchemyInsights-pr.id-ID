---
title: Akses layanan pensiun
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 977bd5887ef58b328463a9befcd6b47ac55f5a85
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687261"
---
# <a name="access-services-retirement"></a>Akses layanan pensiun

Seperti yang kita awalnya diumumkan di MC97576, pada bulan Maret 2017, dan terus berkomunikasi selama tahun lalu layanan akses sedang pensiun. Tahap berikutnya dalam proses ini akan penghapusan akses web database yang menggunakan daftar SharePoint sebagai penyimpanan data dasar mereka.

**Bagaimana hal ini mempengaruhi saya?**

Mulai 2019 Juni, kami akan menghentikan pembuatan database Access baru di SharePoint online dan menutup layanan dan aplikasi yang tersisa dengan 2020 April.

**Apa yang harus saya lakukan untuk mempersiapkan perubahan ini?**

Kami mendorong Anda untuk membuat rencana transisi untuk database web akses organisasi Anda. Admin dapat menggunakan [pemindai aplikasi SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) untuk mendapatkan inventaris aplikasi Access yang menggunakan situs.

Ada beberapa cara untuk bermigrasi akses data web database:

- Mengimpor ke pangkalan data akses lokal (. ACCDB) atau ke file Excel.
- Kami juga menyarankan untuk menjelajahi Microsoft PowerApps sebagai platform alternatif untuk membuat solusi bisnis tanpa kode untuk perangkat seluler dan web.