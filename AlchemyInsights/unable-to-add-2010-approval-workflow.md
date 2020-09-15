---
title: Tidak dapat menambahkan 2010 persetujuan alur kerja
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: aa61f1615b60d27cffad15f02f6ce5dbac1b607f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47699738"
---
# <a name="unable-to-add-2010-approval-workflow"></a>Tidak dapat menambahkan 2010 persetujuan alur kerja

Dalam kumpulan situs Microsoft SharePoint, Anda tidak bisa menambahkan alur kerja yang dapat digunakan kembali secara global (seperti "persetujuan-SharePoint 2010") ke daftar atau pustaka.
  
Untuk mengatasi masalah ini, ikuti langkah-langkah berikut: 
  
1. Buka situs web akar kumpulan situs di SharePoint Designer 2013.
  
2. Di bawah **objek situs**, pilih **alur kerja**. 
  
3. Di bagian **baru** pita **alur kerja** , pilih **alur kerja yang dapat digunakan kembali**. 
  
4. Pada formulir **buat alur kerja yang dapat digunakan kembali** , masukkan nama * * *Repair2010* * *. Untuk **tipe platform**, klik **alur kerja SharePoint 2010**, lalu klik **OK**. 
  
1. Di bagian **Simpan** pada pita **alur kerja** , pilih **terbitkan**. 
  
2. Di bagian **Kelola** dari pita **alur kerja** , pilih **terbitkan secara global**. Dalam kotak dialog konfirmasi yang muncul, pilih **OK**. 
  
3. Di browser web, temukan situs web akar dari kumpulan situs, lalu akses **Site Settings** \> **fitur kumpulan situs**pengaturan situs. Mengaktifkan fitur **alur kerja** : 
  
· Jika fitur  *diaktifkan*  , klik **Nonaktifkan,** lalu klik **Aktifkan**. 
  
· Jika fitur  *dinonaktifkan*  , klik **Aktifkan**. 
  
Untuk informasi selengkapnya, lihat [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)berikut ini.
  

