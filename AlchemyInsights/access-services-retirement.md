---
title: Pensiun Layanan Access
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698685"
---
# <a name="access-services-retirement"></a>Pensiun Layanan Access

Seperti yang kami Umumkan di MC97576, pada bulan Maret 2017, dan melanjutkan untuk berkomunikasi selama tahun lalu Layanan Access telah dihentikan. Fase berikutnya dalam proses ini adalah penghapusan database Web Access yang menggunakan daftar SharePoint sebagai penyimpanan data yang mendasari.

**Bagaimana hal ini mempengaruhi saya?**

Mulai 2019 Juni, kami akan menghentikan pembuatan database Access baru di SharePoint online dan menutup layanan dan aplikasi yang tersisa pada bulan April 2020.

**Apa yang perlu saya lakukan untuk mempersiapkan perubahan ini?**

Kami menyarankan agar Anda membuat rencana transisi untuk database Web Access organisasi Anda. Admin dapat menggunakan [pemindai aplikasi akses SharePoint](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) untuk mendapatkan inventaris aplikasi Access yang digunakan situs.

Ada beberapa cara untuk melakukan migrasi data database Web Access:

- Mengimpor ke database Access lokal (. ACCDB) atau ke file Excel.
- Kami juga merekomendasikan menjelajahi Microsoft PowerApps sebagai platform alternatif untuk membuat solusi bisnis tanpa kode untuk perangkat web dan seluler.