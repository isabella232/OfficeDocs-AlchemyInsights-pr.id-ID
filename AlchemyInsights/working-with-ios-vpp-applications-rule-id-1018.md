---
title: Bekerja dengan iOS VPP aplikasi aturan id 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 88a1ef66bf337b3a0094976c122330591aee77ff
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719960"
---
# <a name="working-with-ios-vpp-applications"></a>Bekerja dengan aplikasi iOS VPP

Baca [cara mengelola aplikasi IOS yang dibeli melalui program pembelian volume dengan Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) untuk mempelajari tentang fitur, kendala, dan langkah untuk memanfaatkan program pembelian volume Apple dan dukungan untuk itu di Microsoft Intune.
  
 **Masalah umum:** "Saya menugaskan aplikasi iOS VPP ke pengguna saya, namun penginstalan gagal."
  
- Hal ini dapat terjadi jika Token VPP tunggal digunakan di beberapa penyedia manajemen perangkat seluler. Token VPP dari Apple hanya dapat digunakan dengan satu penyedia. Jika Anda menggunakan token VPP dengan beberapa penyedia, Anda harus kembali meng-upload token ke Intune.

- Penginstalan juga dapat gagal jika jumlah total penginstalan melebihi jumlah lisensi. Untuk melihat laporan penggunaan untuk lisensi Anda, buka halaman \> **lisensi aplikasi** **aplikasi seluler Intune** . Untuk mempelajari cara merebut kembali lisensi yang digunakan, lihat [artikel ini.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
