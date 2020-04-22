---
title: Alur kerja hilang gagal Aktifkan
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 2598111005c219c398b63ca374e8e99348efc02c
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43762104"
---
# <a name="missing-workflow-failed-to-activate"></a>Alur kerja hilang gagal Aktifkan

Dalam koleksi situs Microsoft SharePoint, Anda tidak dapat menambahkan alur kerja global Reusable (seperti "persetujuan-SharePoint 2010") ke daftar atau Perpustakaan.
  
Untuk mengatasi masalah ini, ikuti langkah berikut: 
  
1. Buka situs akar koleksi situs di 2013 SharePoint Designer.
  
2. Di bawah **objek situs**, pilih **alur kerja**. 
  
3. Di bagian **baru** pita **alur kerja** , pilih **alur kerja dapat digunakan kembali**. 
  
4. Pada formulir **buat alur kerja yang dapat digunakan kembali** , masukkan nama * * *Repair2010* * *. Untuk **jenis platform**, klik **alur kerja SharePoint 2010**, dan kemudian klik **OK**. 
  
1. Di bagian **Simpan** pita **alur kerja** , pilih **terbitkan**. 
  
2. Di bagian **Kelola** pita **alur kerja** , pilih **terbitkan secara global**. Di kotak dialog konfirmasi yang muncul, pilih **OK**. 
  
3. Di web browser, temukan situs akar koleksi situs, dan kemudian akses **situs pengaturan** \> **situs koleksi fitur**. Kemudian, beralih fitur **alur kerja** : 
  
· Jika fitur *diaktifkan* , klik **Nonaktifkan,** dan kemudian klik **Aktifkan**. 
  
· Jika fitur *dinonaktifkan* , klik **Aktifkan**. 
  
Untuk informasi lebih lanjut, silakan merujuk ke [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)berikut.
  

