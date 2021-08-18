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
ms.openlocfilehash: a0f48dc79b51168c9cc045078ad8fc7d668343c7
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327605"
---
# <a name="modern-site-as-root-site"></a>Situs modern sebagai situs akar

Kami telah mulai meluncurkan fitur baru yang akan memungkinkan Anda menukar situs akar [situs klasik dengan situs modern.](https://docs.microsoft.com/sharepoint/modern-root-site) Gunakan [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) untuk menukar lokasi situs dengan situs lain sambil mengarsipkan situs aslinya. Tersedia untuk Situs Tim (tidak tersambung ke grup) dan Situs Komunikasi.

**Penting**: Jangan menghapus situs akar klasik Anda untuk membuat Situs Komunikasi modern. Hal ini tidak didukung oleh Microsoft. Menghapus situs akar akan membuat semua SharePoint situs di organisasi Anda tidak dapat diakses oleh semua pengguna, hingga Anda memulihkan situs atau membuat situs baru di URL yang sama. Kami akan mengomunikasikan fitur ini melalui pusat pesan. Sebaiknya fitur segera diaktifkan dalam penyewa Anda.

## <a name="known-issues-with-swapping-sites"></a>Masalah umum dalam menukar situs
- Situs target mungkin mengembalikan kesalahan "tidak ditemukan" (HTTP 404) untuk jangka waktu yang singkat.
- Konten harus digambar ulang untuk memperbarui indeks pencarian. Tidak ada langkah manual yang diperlukan di sini, ini akan dilakukan secara otomatis.
- Apa pun yang bergantung pada link "statis" (seperti Sinkronisasi File OneNote file) harus diperbaiki secara manual.
- Project Situs server mungkin harus divalidasi untuk memastikan bahwa situs masih terkait dengan benar. 
