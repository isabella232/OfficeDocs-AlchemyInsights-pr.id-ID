---
title: Situs modern sebagai situs akar
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 0388f95e2b7815dcbbb6aca200f44e55e9c5724f
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713794"
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
