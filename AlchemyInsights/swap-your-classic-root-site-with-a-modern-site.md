---
title: Swap situs akar klasik dengan sebuah situs Modern
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 0f6f962314d9099bd21c281a23ad2e95742da4a8
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270747"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Swap situs akar klasik dengan sebuah situs Modern

Jika lingkungan Anda mengatur sebelum April 2019, Anda dapat mengubah situs akar Anda ke situs modern dengan menggunakan Microsoft PowerShell:

- Jika Anda memiliki situs yang berbeda yang ingin Anda gunakan sebagai situs akar Anda, Anda dapat mengganti (swap) akar situs dengan itu. 
    - Gunakan [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) untuk menukar lokasi situs dengan situs lain sementara pengarsipan situs asli. Tersedia untuk tim situs (tidak terhubung ke grup) dan komunikasi situs. 

- Kemampuan tambahan akan diperkenalkan segera yang akan memungkinkan Anda untuk tetap menggunakan konten di situs, tetapi mengubah situs yang sudah ada ke situs komunikasi. 
>[!Important]
>Kemampuan ini akan digulirkan secara bertahap. Terus memeriksa pesan 365 kantor pusat untuk update. 

## <a name="known-issues-with-swapping-sites"></a>Masalah yang dikenal dengan menukar situs

- Situs target mungkin kembali "tidak ditemukan" kesalahan (HTTP 404) untuk periode waktu yang singkat.
- Konten akan perlu recrawled untuk memperbarui indeks pencarian. Tidak ada langkah manual yang diperlukan - ini akan dilakukan secara otomatis.
- Apa pun yang bergantung pada "statis" link (seperti File Sync dan OneNote file) akan perlu diperbaiki secara manual.
- Jika situs sumber situs berita organisasi, memperbarui URL.Mendapatkan daftar semua situs berita organisasi.
- Lokasi Server proyek mungkin perlu divalidasi untuk memastikan bahwa mereka masih berhubungan dengan benar.





