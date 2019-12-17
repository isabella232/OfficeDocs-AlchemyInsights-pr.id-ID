---
title: Situs modern sebagai situs akar
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 2e2bb02b9dbaf7f8ede0b4c5ba8c8f29453309cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054705"
---
# <a name="modern-site-as-root-site"></a>Situs modern sebagai situs akar

Kami telah mulai peluncuran fitur baru yang akan memungkinkan Anda untuk [swap situs akar situs klasik Anda dengan situs modern](https://docs.microsoft.com/sharepoint/modern-root-site). Gunakan [invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) untuk menukar lokasi situs dengan situs lain saat pengarsipan situs asli. Tersedia untuk kedua tim situs (tidak terhubung ke grup) dan situs komunikasi.

>[!Important]
> Jangan menghapus situs root klasik Anda untuk membuat situs komunikasi modern. Hal ini tidak didukung oleh Microsoft. Menghapus situs akar akan membuat semua situs SharePoint di organisasi Anda tidak dapat diakses oleh semua pengguna, sampai Anda memulihkan situs atau membuat situs baru di URL yang sama. Kami akan mengkomunikasikan fitur ini melalui pusat pesan. Anda harus mengharapkan fitur yang akan diaktifkan di penyewa Anda segera.

## <a name="known-issues-with-swapping-sites"></a>Masalah yang diketahui dengan swapping Sites
- Situs target dapat mengembalikan galat "tidak ditemukan" (HTTP 404) untuk jangka waktu yang singkat.
- Konten harus di-recrawled untuk memperbarui indeks pencarian. Tidak ada langkah manual yang diperlukan di sini, ini akan dilakukan secara otomatis.
- Apa pun tergantung pada "statis" link (seperti file Sync dan OneNote file) harus dikoreksi secara manual.
- Proyek server situs mungkin perlu divalidasi untuk memastikan bahwa mereka masih terkait dengan benar. 
