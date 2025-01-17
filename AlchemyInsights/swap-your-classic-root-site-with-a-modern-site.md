---
title: Menukar situs akar Klasik Anda dengan situs Modern
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: e8501414498bf1937e98abaca32987e3276bb54e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316143"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Menukar situs akar Klasik Anda dengan situs Modern

Jika lingkungan disiapkan sebelum April 2019, Anda dapat mengubah situs akar ke situs modern menggunakan Microsoft PowerShell:

- Jika memiliki situs lain yang ingin digunakan sebagai situs akar, Anda dapat mengganti [(menukar) situs akar](https://docs.microsoft.com/sharepoint/modern-root-site) dengan situs tersebut. 
    - Gunakan [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) untuk menukar lokasi situs dengan situs lain sambil mengarsipkan situs aslinya. Tersedia untuk Situs Tim (tidak tersambung ke grup) dan Situs Komunikasi. 

- Kapabilitas tambahan akan segera diperkenalkan yang akan memungkinkan Anda untuk terus menggunakan konten di situs, tapi mengonversi situs yang sudah ada ke situs komunikasi. 

**Penting**: Kemampuan ini akan diluncurkan secara bertahap. Lanjutkan untuk memeriksa Pusat Pesan untuk pembaruan. 

## <a name="known-issues-with-swapping-sites"></a>Masalah umum dalam menukar situs

- Situs target mungkin mengembalikan kesalahan "tidak ditemukan" (HTTP 404) untuk jangka waktu yang singkat.
- Konten harus digambar ulang untuk memperbarui indeks pencarian. Tidak diperlukan langkah manual - ini akan dilakukan secara otomatis.
- Apa pun yang bergantung pada link "statis" (seperti Sinkronisasi File OneNote file) harus diperbaiki secara manual.
- Jika situs sumber adalah situs berita organisasi, perbarui URL. Dapatkan daftar semua situs berita organisasi.
- Project Situs server mungkin harus divalidasi untuk memastikan bahwa situs masih terkait dengan benar.
