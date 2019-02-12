---
title: Buka dengan Explorer tidak bekerja
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: f788c3c626cdeb19970edb59563c59eea60e2992
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/12/2019
ms.locfileid: "29906807"
---
# <a name="open-with-explorer-isnt-working"></a>Buka dengan Explorer tidak bekerja

Jika **terbuka dengan Explorer** atau **lihat di File Explorer** tidak berfungsi pastikan layanan WebClient diatur untuk **menjalankan** dengan mengikuti langkah-langkah berikut. Sebagai contoh, itu mungkin memakan waktu lama untuk membuka perpustakaan SharePoint atau OneDrive ketika Layanan tidak berjalan. 
  
1. Di kotak pencarian Windows, menjalankan, jenis pilih aplikasi desktop jalankan, ketik services.msc, dan kemudian pilih **Enter**.
    
2. Gulir ke bawah ke layanan WebClient dan memeriksa kolom **Status** . Jika status layanan WebClient tidak **menjalankan**, klik dua kali layanan, klik **mulai**, dan kemudian klik **OK**. Mengaktifkan layanan, jika diperlukan, dengan memilih baik **Manual** atau **otomatis** di kotak **Startup type** . 
    
> [!NOTE]
> Untuk memecahkan masalah membuka File Explorer, lihat [terbuka di Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Jelajahi sync sebagai alternatif yang lebih baik: [Sync SharePoint file dengan OneDrive sync klien baru](https://go.microsoft.com/fwlink/?linkid=871666). 
  

