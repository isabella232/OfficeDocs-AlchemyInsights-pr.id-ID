---
title: Menukar situs akar klasik Anda dengan situs modern
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
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691182"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Menukar situs akar klasik Anda dengan situs modern

Jika lingkungan Anda disiapkan sebelum 2019 April, Anda bisa mengubah situs akar Anda menjadi situs modern dengan menggunakan Microsoft PowerShell:

- Jika Anda memiliki situs yang berbeda yang ingin Anda gunakan sebagai situs akar Anda, Anda bisa mengganti [(bertukar) situs akar](https://docs.microsoft.com/sharepoint/modern-root-site) dengan file tersebut. 
    - Gunakan [invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) untuk menukar lokasi situs dengan situs lain saat mengarsipkan situs asli. Tersedia untuk kedua situs tim (tidak tersambung ke grup) dan situs komunikasi. 

- Kemampuan tambahan akan segera diperkenalkan yang akan memungkinkan Anda untuk tetap menggunakan konten di situs, tapi mengonversi situs yang sudah ada ke situs komunikasi. 
>[!Important]
>Kapabilitas ini akan diluncurkan secara bertahap. Lanjutkan untuk memeriksa pusat pesan untuk pembaruan. 

## <a name="known-issues-with-swapping-sites"></a>Masalah yang diketahui dengan situs bertukar

- Situs target mungkin mengembalikan kesalahan "tidak ditemukan" (HTTP 404) untuk periode waktu yang singkat.
- Konten harus diberi kembali untuk memperbarui indeks pencarian. Tidak diperlukan langkah manual-ini akan dilakukan secara otomatis.
- Apa pun yang bergantung pada tautan "statis" (seperti file sinkronisasi file dan OneNote) perlu dikoreksi secara manual.
- Jika situs sumber merupakan situs berita organisasi, perbarui URL.Dapatkan daftar semua situs berita organisasi.
- Situs Project Server mungkin perlu divalidasi untuk memastikan bahwa situs tersebut masih terkait dengan benar.
