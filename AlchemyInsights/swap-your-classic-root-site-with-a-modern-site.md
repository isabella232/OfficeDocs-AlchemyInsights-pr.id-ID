---
title: Swap situs root Classic Anda dengan situs modern
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
ms.openlocfilehash: bd477d90ab7e6737aafffc57d931aad2bd0351e8
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/04/2019
ms.locfileid: "36749263"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Swap situs root Classic Anda dengan situs modern

Jika lingkungan Anda diatur sebelum 2019 April, Anda dapat mengubah situs akar Anda ke situs modern dengan menggunakan Microsoft PowerShell:

- Jika Anda memiliki situs yang berbeda yang ingin Anda gunakan sebagai situs akar Anda, Anda dapat mengganti [(swap) situs akar](https://docs.microsoft.com/sharepoint/modern-root-site) dengan itu. 
    - Gunakan [invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) untuk menukar lokasi situs dengan situs lain saat pengarsipan situs asli. Tersedia untuk kedua tim situs (tidak terhubung ke grup) dan situs komunikasi. 

- Kemampuan tambahan akan diperkenalkan segera yang akan memungkinkan Anda untuk tetap menggunakan konten di situs, tetapi mengkonversi situs yang ada ke situs komunikasi. 
>[!Important]
>Kemampuan ini akan diluncurkan secara bertahap. Lanjutkan untuk memeriksa Office 365 message Center untuk pembaruan. 

## <a name="known-issues-with-swapping-sites"></a>Masalah yang diketahui dengan swapping Sites

- Situs target dapat mengembalikan galat "tidak ditemukan" (HTTP 404) untuk jangka waktu yang singkat.
- Konten harus di-recrawled untuk memperbarui indeks pencarian. Tidak ada langkah manual yang diperlukan-ini akan dilakukan secara otomatis.
- Apa pun tergantung pada "statis" link (seperti file Sync dan OneNote file) harus dikoreksi secara manual.
- Jika situs sumber adalah situs berita organisasi, perbarui URL.Dapatkan daftar semua situs berita organisasi.
- Proyek server situs mungkin perlu divalidasi untuk memastikan bahwa mereka masih terkait dengan benar.





