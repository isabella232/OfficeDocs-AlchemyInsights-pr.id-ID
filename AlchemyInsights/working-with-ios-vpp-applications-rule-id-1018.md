---
title: Bekerja dengan Id Aturan Aplikasi VPP iOS 1018
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
ms.openlocfilehash: f693d12ff0f9c193cba0c6a6802b22d7acd37532c65986e5f6613e18c021f06b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083017"
---
# <a name="working-with-ios-vpp-applications"></a>Bekerja dengan Aplikasi VPP iOS

Baca Cara mengelola aplikasi iOS yang dibeli melalui program pembelian volume dengan Microsoft Intune untuk mempelajari tentang fitur, batasan, dan [langkah-langkah](https://docs.microsoft.com/intune/vpp-apps-ios) untuk menggunakan Program Pembelian Volume Apple dan dukungan untuk aplikasi di Microsoft Intune.
  
 **Masalah Umum:** "Saya menetapkan aplikasi VPP iOS ke pengguna saya, tetapi penginstalan gagal."
  
- Hal ini dapat terjadi jika satu token VPP digunakan di beberapa penyedia manajemen perangkat seluler. Token VPP dari Apple hanya dapat digunakan dengan satu penyedia. Jika Anda menggunakan token VPP dengan beberapa penyedia, Anda harus mengunggah kembali token ke Intune.

- Instalasi juga bisa gagal jika jumlah total instalasi melebihi jumlah lisensi. Untuk menampilkan laporan penggunaan untuk lisensi Anda, buka halaman lisensi Aplikasi **Seluler Intune.** \>  Untuk mempelajari cara mengklaim kembali lisensi yang digunakan, lihat [artikel ini.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
