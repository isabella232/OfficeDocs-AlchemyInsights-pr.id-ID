---
title: Alur Kerja Hilang Gagal Diaktifkan
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: d703e87f355f05bf4a1d71e5daddce96db988380bb48accc81c95f1ba91fbb2b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54065431"
---
# <a name="missing-workflow-failed-to-activate"></a>Alur Kerja Hilang Gagal Diaktifkan

Dalam kumpulan situs Microsoft SharePoint, Anda tidak dapat menambahkan alur kerja yang dapat digunakan kembali secara global (seperti "Persetujuan - SharePoint 2010") ke daftar atau pustaka.
  
Untuk mengatasi masalah ini, ikuti langkah-langkah berikut: 
  
1. Buka situs web akar kumpulan situs di SharePoint Designer 2013.
  
2. Di **bawah Objek Situs,** pilih **Alur Kerja.** 
  
3. Di bagian **Baru** pita Alur **Kerja,** pilih Alur Kerja yang Dapat **Digunakan Kembali.** 
  
4. Pada formulir **Buat Alur Kerja yang Dapat** Digunakan Kembali, masukkan nama ** *Repair2010* **. Untuk **Tipe Platform,** klik **SharePoint Alur Kerja 2010,** lalu klik **OK.** 
  
1. Di bagian **Simpan** pada pita Alur **Kerja,** pilih **Terbitkan.** 
  
2. Di bagian **Kelola** pada pita **Alur Kerja,** pilih **Terbitkan Secara Global.** Dalam kotak dialog konfirmasi yang muncul, pilih **OK.** 
  
3. Di browser web, temukan akar situs web kumpulan situs, lalu akses Situs **Pengaturan** \> **Kumpulan Situs**. Lalu, alihkan **fitur Alur** Kerja: 
  
· Jika fitur *diaktifkan, klik* **Nonaktifkan,** lalu klik **Aktifkan.** 
  
· Jika fitur *Dinonaktifkan,* klik **Aktifkan.** 
  
Untuk informasi selengkapnya, silakan lihat artikel [berikut ini](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

