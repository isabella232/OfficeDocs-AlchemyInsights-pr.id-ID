---
title: Situs modern sebagai situs akar
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666873"
---
# <a name="modern-site-as-root-site"></a>Situs modern sebagai situs akar

Kami telah mulai meluncurkan fitur baru yang akan memungkinkan Anda untuk [menukar situs root situs klasik Anda dengan situs modern](https://docs.microsoft.com/sharepoint/modern-root-site). Gunakan [invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) untuk menukar lokasi situs dengan situs lain saat mengarsipkan situs asli. Tersedia untuk kedua situs tim (tidak tersambung ke grup) dan situs komunikasi.

>[!Important]
> Jangan menghapus situs akar klasik Anda untuk membuat situs komunikasi modern. Ini tidak didukung oleh Microsoft. Menghapus situs akar akan membuat semua situs SharePoint di organisasi Anda tidak dapat diakses oleh semua pengguna, hingga Anda memulihkan situs atau membuat situs baru di URL yang sama. Kami akan mengkomunikasikan fitur ini melalui pusat pesan. Anda akan diminta untuk mengaktifkan fitur dalam penyewa Anda.

## <a name="known-issues-with-swapping-sites"></a>Masalah yang diketahui dengan situs bertukar
- Situs target mungkin mengembalikan kesalahan "tidak ditemukan" (HTTP 404) untuk periode waktu yang singkat.
- Konten harus diberi kembali untuk memperbarui indeks pencarian. Tidak ada langkah manual yang diperlukan di sini, ini akan dilakukan secara otomatis.
- Apa pun yang bergantung pada tautan "statis" (seperti file sinkronisasi file dan OneNote) perlu dikoreksi secara manual.
- Situs Project Server mungkin perlu divalidasi untuk memastikan bahwa situs tersebut masih terkait dengan benar. 
