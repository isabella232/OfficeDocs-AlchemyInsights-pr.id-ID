---
title: Terbuka dengan Explorer tidak bekerja
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: dc939a3451ff4fe95e4aa5a999839a2c532b398c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713037"
---
# <a name="open-with-explorer-isnt-working"></a>Buka dengan penjelajah tidak bekerja

Jika **buka dengan Explorer** atau **lihat di file Explorer** tidak bekerja pastikan bahwa layanan WebClient diatur untuk **menjalankan** dengan mengikuti langkah di bawah ini. Sebagai contoh, mungkin membutuhkan waktu lama untuk membuka perpustakaan SharePoint atau OneDrive ketika Layanan tidak berjalan. 
  
1. Di kotak pencarian Windows, ketik jalankan, pilih Jalankan aplikasi desktop, ketik Services. MSC, dan kemudian pilih **Enter**.
    
2. Gulir ke bawah ke layanan WebClient dan periksa kolom **status** . Jika status layanan WebClient tidak **berjalan**, klik dua kali layanan, klik **mulai**, dan kemudian klik **OK**. Aktifkan layanan, jika diperlukan, dengan memilih salah satu **manual** atau **otomatis** di kotak **jenis startup** . 
    
> [!NOTE]
> Untuk memecahkan masalah pembukaan di file Explorer, lihat [buka di Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Jelajahi sinkronisasi sebagai alternatif yang lebih baik: [menyinkronkan berkas SharePoint dengan klien sinkronisasi OneDrive baru](https://go.microsoft.com/fwlink/?linkid=871666). 
  

