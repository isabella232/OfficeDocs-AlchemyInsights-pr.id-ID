---
title: Akses ditolak saat melihat alur kerja
ms.author: pebaum
author: pebaum
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 1cfda8e08ada05858a28f2bede8c31261f9de351
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050528"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Akses ditolak saat melihat alur kerja

SharePoint 2013 alur kerja yang mencoba mengirim email ke grup SharePoint dapat gagal dengan pesan galat "Akses ditolak" Jika keanggotaan grup SharePoint tidak ditetapkan ke semua orang.
  
 **Untuk mengatasi masalah ini, lakukan langkah berikut:**
  
 1. Izinkan semua orang untuk melihat anggota kelompok SharePoint.
  
 2. Hapus grup SharePoint dari baris kepada atau CC email.
  
 3. Secara eksplisit menambahkan pengguna ke baris kepada atau CC jika visibilitas keanggotaan tidak dapat diubah untuk grup SharePoint.
  
Untuk melihat rincian lebih lanjut silakan merujuk ke [http tidak sah untuk/_vti_bin/client.SVC/SP.Utilities.Utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  