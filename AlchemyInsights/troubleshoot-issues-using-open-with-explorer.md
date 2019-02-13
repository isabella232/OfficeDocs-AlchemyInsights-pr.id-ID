---
title: Memecahkan masalah menggunakan terbuka dengan Explorer
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 9b2abe01a47d39812988d62b6f010a8933fad33e
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/12/2019
ms.locfileid: "29929211"
---
# <a name="fix-problems-with-open-with-explorer"></a>Memperbaiki masalah dengan terbuka dengan Explorer

Memperbaiki masalah umum dengan membuka pustaka dokumen di SharePoint atau OneDrive menggunakan perintah **terbuka dengan Explorer** : 
  
- Gunakan Internet Explorer 10 atau Internet Explorer 11. **Terbuka dengan Explorer** tidak kompatibel dengan Microsoft Edge, Google Chrome, Firefox, dan lain-lain. **Terbuka dengan Explorer** dinonaktifkan di semua browser kecuali Internet Explorer. 
    
- **Terbuka dengan Explorer** ini tidak tersedia dalam pengalaman modern untuk SharePoint Perpustakaan. Menggunakan **tampilan di File Explorer** sebagai gantinya. Pilih **opsi tampilan** \> **pandangan dalam File Explorer**. Lihat di File Explorer tidak kompatibel dengan Microsoft Edge, Google Chrome, Firefox, dan lain-lain. **Tampilan di File Explorer** di tersedia hanya di Internet Explorer. 
    
- Pastikan Layanan WebClient berjalan. Di kotak pencarian Windows, ketik dijalankan, pilih aplikasi desktop jalankan, ketik services.msc, dan kemudian tekan Enter. Gulir ke bawah untuk WebClient layanan dan pastikan kolom **Status** menampilkan "Berjalan." Jika tidak, klik dua kali layanan, klik **mulai**, dan kemudian klik **OK**. (Anda mungkin perlu terlebih dahulu mengaktifkan layanan dengan memilih baik **Manual** atau **otomatis** di kotak **Startup type** .) 
    
> [!NOTE]
> Membuka sebuah perpustakaan di File Explorer berguna jika Anda perlu untuk menyalin atau memindahkan beberapa file dan folder sekali, tetapi jika Anda ingin secara teratur bekerja di Perpustakaan, sebaiknya sinkronisasi. Untuk memecahkan masalah membuka File Explorer, lihat [terbuka di Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Untuk info tentang cara mengatur sinkronisasi, lihat [Sync SharePoint file dengan OneDrive sync klien baru](https://go.microsoft.com/fwlink/?linkid=871666).
  
Silakan lihat artikel [bagaimana menggunakan perintah "terbuka dengan Explorer" untuk memecahkan masalah di SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) untuk informasi lebih lanjut. 
  

