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
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694459"
---
# <a name="open-with-explorer-isnt-working"></a>Buka dengan Explorer tidak berfungsi

Jika **buka dengan Explorer** atau **tampilan di file Explorer** tidak berfungsi, pastikan layanan WebClient diatur agar **berjalan** dengan mengikuti langkah-langkah di bawah ini. Misalnya, mungkin memerlukan waktu lama untuk membuka pustaka SharePoint atau OneDrive saat Layanan tidak berjalan. 
  
1. Dalam kotak pencarian Windows, ketik jalankan, pilih Jalankan aplikasi desktop, ketikkan Services. MSC, lalu pilih **Enter**.
    
2. Gulir ke bawah ke layanan WebClient dan periksa kolom **status** . Jika status layanan WebClient tidak **berjalan**, klik ganda Layanan tersebut, klik **mulai**, lalu klik **OK**. Aktifkan layanan, jika diperlukan, dengan memilih **manual** atau **otomatis** dalam kotak **tipe startup** . 
    
> [!NOTE]
> Untuk memecahkan masalah yang dibuka di file Explorer, lihat [membuka di Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Jelajahi sinkronisasi sebagai alternatif yang lebih baik: [sinkronkan file SharePoint dengan klien sinkronisasi OneDrive yang baru](https://go.microsoft.com/fwlink/?linkid=871666). 
  

