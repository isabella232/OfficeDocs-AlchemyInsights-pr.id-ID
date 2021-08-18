---
title: Buka dengan Explorer tidak berfungsi
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 2ba6f08b40dd194bf1ffd9a455a134a2fc553b51
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321864"
---
# <a name="open-with-explorer-isnt-working"></a>Buka dengan Explorer tidak berfungsi

Jika **Buka dengan Explorer** atau Tampilkan di File **Explorer** tidak berfungsi pastikan layanan WebClient diatur ke Berjalan dengan mengikuti **langkah-langkah** di bawah ini. Misalnya, mungkin akan memakan waktu lama untuk membuka pustaka SharePoint OneDrive atau saat layanan tidak berjalan. 
  
1. Dalam kotak Windows pencarian, ketikkan jalankan, pilih aplikasi desktop Jalankan, ketik services.msc, lalu pilih **Enter**.
    
2. Gulir ke bawah ke layanan WebClient dan periksa **kolom Status.** Jika status layanan WebClient tidak **Berjalan,** klik ganda layanan, klik **Mulai,** lalu klik **OK.** Aktifkan layanan, jika diperlukan, dengan memilih **Manual atau** **Otomatis dalam** kotak **Tipe mulai.** 
    
**Catatan**: Untuk memecahkan masalah saat membuka di File Explorer, lihat [Membuka di Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Jelajahi sinkronisasi sebagai alternatif yang lebih [baik: Sinkronkan SharePoint file dengan klien OneDrive Sync baru.](https://go.microsoft.com/fwlink/?linkid=871666) 
  

