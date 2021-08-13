---
title: Layanan Access akan pensiun
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
ms.openlocfilehash: 32da879de230dc0ed99563ad881ab5b2479b8453933a127961a26d619e108ab9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53938698"
---
# <a name="access-services-retirement"></a>Layanan Access akan pensiun

Seperti yang telah kami sampaikan sebelumnya di MC97576, pada Maret 2017, dan terus berkomunikasi selama beberapa tahun Layanan Access akan dihentikan. Fase berikutnya dalam proses ini akan menjadi penghapusan Database Web Access yang menggunakan daftar SharePoint sebagai penyimpanan data yang mendasarinya.

**Bagaimana hal ini memengaruhi saya?**

Mulai Juni 2019, kami akan menghentikan pembuatan database Access baru di SharePoint Online dan mematikan layanan serta aplikasi lainnya pada April 2020.

**Apa yang perlu saya lakukan untuk mempersiapkan perubahan ini?**

Kami menyarankan Anda untuk membuat rencana transisi untuk database web Access organisasi. Admin dapat menggunakan [SharePoint pemindai aplikasi Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) untuk mendapatkan inventaris dari aplikasi Access yang digunakan oleh situs.

Ada beberapa cara untuk melakukan migrasi data database web Access:

- Mengimpor ke database Access lokal (. ACCDB) atau ke Excel anda.
- Kami juga menyarankan Microsoft PowerApps sebagai platform alternatif untuk membuat solusi bisnis tanpa kode bagi perangkat seluler dan web.