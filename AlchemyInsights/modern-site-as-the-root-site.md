---
title: Situs modern sebagai situs akar
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 2f75f1e60af06da47fe846e84bbb370dd60084e9
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36543856"
---
# <a name="modern-site-as-root-site"></a>Situs modern sebagai situs akar

Kami telah mulai untuk peluncuran fitur baru yang akan memungkinkan Anda untuk menukar situs akar klasik situs Anda dengan situs modern. Gunakan [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) untuk menukar lokasi situs dengan situs lain sementara pengarsipan situs asli. Tersedia untuk tim situs (tidak terhubung ke grup) dan komunikasi situs. 

>[!Important]
> Tidak menghapus situs akar klasik untuk membuat situs komunikasi modern. Hal ini tidak didukung oleh Microsoft. Menghapus situs akar akan membuat semua situs SharePoint dalam organisasi Anda tidak dapat diakses untuk semua pengguna, sampai Anda mengembalikan situs atau membuat situs baru di URL yang sama. Kita akan berkomunikasi melalui pusat pesan fitur ini. Anda harus mengharapkan fitur harus diaktifkan di penyewa Anda segera.

## <a name="known-issues-with-swapping-sites"></a>Masalah yang dikenal dengan menukar situs
- Situs target mungkin kembali "tidak ditemukan" kesalahan (HTTP 404) untuk periode waktu yang singkat.
- Konten akan perlu recrawled untuk memperbarui indeks pencarian. Tidak ada langkah manual yang diperlukan di sini, ini akan dilakukan secara otomatis.
- Apa pun yang bergantung pada "statis" link (seperti File Sync dan OneNote file) akan perlu diperbaiki secara manual.
- Lokasi Server proyek mungkin perlu divalidasi untuk memastikan bahwa mereka masih berhubungan dengan benar. 
