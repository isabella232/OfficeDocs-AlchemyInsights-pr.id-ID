---
title: Tidak dapat menambahkan default penyetelan 2010
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2060c9a1-e714-4d93-925e-629c82c35986
ms.openlocfilehash: 758b0339b842478f9609eb716b5b4ddab6579c80
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/24/2019
ms.locfileid: "29474257"
---
# <a name="cant-add-default-2010-approval-workflow"></a>Tidak dapat menambahkan default penyetelan 2010

Di Microsoft SharePoint situs koleksi, Anda tidak dapat menambahkan alur kerja global dapat digunakan kembali (seperti "persetujuan - SharePoint 2010") ke daftar atau Perpustakaan.
  
Untuk mengatasi masalah ini, ikuti langkah berikut: 
  
1. Buka situs akar koleksi situs di SharePoint desainer 2013.
  
2. **Benda-benda situs**, pilih **alur kerja**. 
  
3. Di bagian **baru** dari pita **alur kerja** , pilih **Reusable alur kerja**. 
  
4. Pada bentuk **Membuat Reusable alur kerja** , masukkan nama * **Repair2010***. Untuk **Jenis Platform**, pilih **SharePoint 2010 alur kerja**, dan kemudian pilih **OK**. 
  
5. Di bagian **menyimpan** pita **alur kerja** , pilih **Publish**. 
  
6. Di bagian **Manage** pita **alur kerja** , pilih **Mempublikasikan secara global**. Di kotak dialog konfirmasi yang muncul, pilih **OK**. 
  
7. Di web browser, mencari situs situs koleksi akar, dan mengakses **Pengaturan situs** \> **Situs koleksi fitur**. Kemudian, beralih fitur **alur kerja** : 
  
· Jika fitur *aktif* , klik **Nonaktifkan,** dan kemudian klik **Aktifkan**. 
  
· Jika fitur *Deactivated* , klik **Aktifkan**. 
  
Untuk informasi lebih lanjut silakan lihat berikut [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

