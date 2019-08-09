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
ms.openlocfilehash: 260048db6c439183da8e0bb0c2dfa3c7475fca79
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/09/2019
ms.locfileid: "36269379"
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
