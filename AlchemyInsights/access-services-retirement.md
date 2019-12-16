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
ms.openlocfilehash: cb8123583b68e945ef878fdbaf211fd1d8205bb3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050492"
---
# <a name="access-services-retirement"></a>Akses layanan pensiun

Seperti yang kita awalnya diumumkan di MC97576, pada Maret 2017, dan terus berkomunikasi selama tahun lalu layanan akses sedang pensiun dari 365 Office. Tahap berikutnya dalam proses ini akan penghapusan akses web database yang menggunakan daftar SharePoint sebagai penyimpanan data dasar mereka.

**Bagaimana hal ini mempengaruhi saya?**

Mulai 2019 Juni, kami akan menghentikan pembuatan database Access baru di SharePoint online dan menutup layanan dan aplikasi yang tersisa dengan 2020 April.

**Apa yang harus saya lakukan untuk mempersiapkan perubahan ini?**

Kami mendorong Anda untuk membuat rencana transisi untuk database web akses organisasi Anda. Admin dapat menggunakan [pemindai aplikasi SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) untuk mendapatkan inventaris aplikasi Access yang menggunakan situs.

Ada beberapa cara untuk bermigrasi akses data web database:

- Mengimpor ke pangkalan data akses lokal (. ACCDB) atau ke file Excel.
- Kami juga menyarankan untuk menjelajahi Microsoft PowerApps sebagai platform alternatif untuk membuat solusi bisnis tanpa kode untuk perangkat seluler dan web.