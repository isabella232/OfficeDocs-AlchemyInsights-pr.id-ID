---
title: Alur kerja hilang gagal Aktifkan
ms.author: pebaum
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: f03d7e1441465050c4b0608f4100f217b183d2e2
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/04/2019
ms.locfileid: "36753799"
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
  

