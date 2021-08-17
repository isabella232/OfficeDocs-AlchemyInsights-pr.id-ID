---
title: Memecahkan masalah penggunaan Buka dengan Explorer
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 0cbcfb506295d5732f7109be7a103bbdef530a529c7408c6d9d45a7b38a89915
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54048159"
---
# <a name="fix-problems-with-open-with-explorer"></a>Memperbaiki masalah dengan Buka dengan Explorer

Perbaiki masalah umum dengan membuka pustaka dokumen di SharePoint atau OneDrive menggunakan **perintah Buka dengan Explorer:** 
  
- Gunakan Internet Explorer 10 atau Internet Explorer 11. **Buka dengan Explorer** tidak kompatibel dengan Microsoft Edge, Google Chrome, Firefox, dan lainnya. **Buka dengan Explorer** dinonaktifkan di semua browser kecuali Internet Explorer. 
    
- **Buka dengan Explorer** tidak tersedia di pengalaman modern untuk SharePoint pustaka. Gunakan **Tampilan di File Explorer** sebagai gantinya. Pilih **Tampilan opsi** Tampilkan di File \> **Explorer.** Tampilan di File Explorer tidak kompatibel dengan Microsoft Edge, Google Chrome, Firefox, dan lainnya. **Menampilkan di File Explorer** hanya tersedia di Internet Explorer. 
    
- Pastikan layanan WebClient sedang berjalan. Dalam kotak Windows pencarian, ketikkan jalankan, pilih aplikasi desktop Jalankan, ketik services.msc, lalu tekan Enter. Gulir ke bawah ke layanan WebClient dan pastikan kolom **Status** menampilkan "Berjalan." Jika tidak, klik ganda layanan, klik **Mulai,** lalu klik **OK.** (Anda mungkin perlu mengaktifkan layanan terlebih dahulu dengan memilih **Manual** atau **Otomatis dalam** kotak **Tipe mulai.)** 
    
> [!NOTE]
> Membuka pustaka di File Explorer akan sangat praktis jika Anda perlu menyalin atau memindahkan beberapa file dan folder sekali, tetapi jika ingin bekerja secara rutin dalam pustaka, sebaiknya sinkronkan pustaka. Untuk memecahkan masalah saat membuka di File Explorer, lihat [Membuka di Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Untuk informasi tentang menyiapkan sinkronisasi, lihat [Menyinkronkan SharePoint file dengan klien OneDrive Sync baru.](https://go.microsoft.com/fwlink/?linkid=871666)
  
Silakan lihat artikel [Cara menggunakan perintah "Buka dengan Explorer"](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) untuk memecahkan masalah dalam SharePoint Online untuk informasi selengkapnya. 
  

