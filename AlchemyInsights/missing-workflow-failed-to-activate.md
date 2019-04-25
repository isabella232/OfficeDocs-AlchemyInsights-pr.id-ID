---
title: Hilang alur kerja gagal untuk mengaktifkan
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: ce088227a3206fa05b99331fdb022fbe4886203f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/23/2019
ms.locfileid: "32418436"
---
# <a name="missing-workflow-failed-to-activate"></a>Hilang alur kerja gagal untuk mengaktifkan

Di Microsoft SharePoint situs koleksi, Anda tidak dapat menambahkan alur kerja global dapat digunakan kembali (seperti "persetujuan - SharePoint 2010") ke daftar atau Perpustakaan.
  
Untuk mengatasi masalah ini, ikuti langkah berikut: 
  
1. Buka situs akar koleksi situs di SharePoint desainer 2013.
  
2. **Benda-benda situs**, pilih **alur kerja**. 
  
3. Di bagian **baru** dari pita **alur kerja** , pilih **Reusable alur kerja**. 
  
4. Pada bentuk **Membuat Reusable alur kerja** , masukkan nama ** *Repair2010* **. Untuk **Jenis Platform**, klik **SharePoint 2010 alur kerja**, dan kemudian klik **OK**. 
  
1. Di bagian **menyimpan** pita **alur kerja** , pilih **Publish**. 
  
2. Di bagian **Manage** pita **alur kerja** , pilih **Mempublikasikan secara global**. Di kotak dialog konfirmasi yang muncul, pilih **OK**. 
  
3. Di web browser, mencari situs situs koleksi akar, dan mengakses **Pengaturan situs** \> **Situs koleksi fitur**. Kemudian, beralih fitur **alur kerja** : 
  
· Jika fitur *aktif* , klik **Nonaktifkan,** dan kemudian klik **Aktifkan**. 
  
· Jika fitur *Deactivated* , klik **Aktifkan**. 
  
Untuk informasi lebih lanjut silakan lihat berikut [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

