---
title: Bekerja dengan iOS VPP aplikasi aturan Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 65b9a727171a7551068717f6327f15e1aa8e6bed
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420487"
---
# <a name="working-with-ios-vpp-applications"></a>Bekerja dengan iOS aplikasi VPP

Baca [bagaimana mengelola aplikasi iOS yang dibeli melalui program volume-pembelian dengan Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) untuk mempelajari tentang fitur, kendala, dan langkah-langkah untuk membuat penggunaan Program membeli Apple Volume dan dukungan untuk itu dalam Microsoft Intune. 
  
 **Masalah umum:** "Aku ditugaskan iOS VPP app untuk pengguna, tetapi instalasi gagal." 
  
- Ini dapat terjadi jika tanda VPP tunggal digunakan di beberapa penyedia manajemen perangkat selular. VPP token dari Apple hanya dapat digunakan dengan salah satu penyedia. Jika Anda menggunakan tanda VPP dengan beberapa penyedia, Anda harus kembali upload token untuk Intune.
    
- Instalasi juga dapat gagal jika jumlah instalasi melebihi jumlah lisensi. Untuk melihat laporan penggunaan untuk lisensi Anda, buka **Intune Mobile apps** \> halaman **App lisensi** . Untuk mempelajari cara untuk merebut kembali lisensi digunakan, lihat [artikel ini.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
    

