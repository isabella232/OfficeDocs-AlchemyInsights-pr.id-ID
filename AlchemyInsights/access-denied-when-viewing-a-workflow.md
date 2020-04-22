---
title: Akses ditolak saat melihat alur kerja
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: c576bf88225582f2577e0b59506a7482cf9f38d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687333"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Akses ditolak saat melihat alur kerja

SharePoint 2013 alur kerja yang mencoba mengirim email ke grup SharePoint dapat gagal dengan pesan galat "Akses ditolak" Jika keanggotaan grup SharePoint tidak ditetapkan ke semua orang.
  
 **Untuk mengatasi masalah ini, lakukan langkah berikut:**
  
 1. Izinkan semua orang untuk melihat anggota kelompok SharePoint.
  
 2. Hapus grup SharePoint dari baris kepada atau CC email.
  
 3. Secara eksplisit menambahkan pengguna ke baris kepada atau CC jika visibilitas keanggotaan tidak dapat diubah untuk grup SharePoint.
  
Untuk melihat rincian lebih lanjut silakan merujuk ke [http tidak sah untuk/_vti_bin/client.SVC/SP.Utilities.Utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  