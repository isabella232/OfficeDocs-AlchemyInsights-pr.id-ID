---
title: Bekerja dengan aturan aplikasi VPP iOS id 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688949"
---
# <a name="working-with-ios-vpp-applications"></a>Bekerja dengan aplikasi iOS VPP

Baca [cara mengelola aplikasi IOS yang dibeli melalui program pembelian-Borongan dengan Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) untuk mempelajari tentang fitur, batasan, dan langkah-langkah untuk memanfaatkan program pembelian di Apple dan dukungan untuk Microsoft Intune.
  
 **Masalah umum:** "Saya menugaskan aplikasi VPP iOS kepada pengguna saya, tapi penginstalan gagal."
  
- Hal ini bisa terjadi jika Token VPP digunakan di beberapa penyedia manajemen perangkat seluler. Token VPP dari Apple hanya dapat digunakan dengan satu penyedia. Jika Anda menggunakan token VPP dengan beberapa penyedia, Anda harus mengunggah ulang token ke Intune.

- Penginstalan juga bisa gagal jika jumlah total instalasi melebihi jumlah lisensi. Untuk menampilkan laporan penggunaan untuk lisensi Anda, buka **Intune Mobile apps** \> halaman **lisensi aplikasi** seluler Intune. Untuk mempelajari cara mendapatkan kembali lisensi yang sedang digunakan, lihat [artikel ini.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
