---
title: Akses ditolak saat melihat alur kerja
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 53bd9285e49e220f880eea21923f261302003127
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36495826"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Akses ditolak saat melihat alur kerja

Workflow 2013 SharePoint yang mencoba untuk mengirim email ke grup SharePoint dapat gagal dengan pesan galat "Akses ditolak" Jika keanggotaan grup SharePoint tidak diset untuk semua orang.
  
 **Untuk mengatasi masalah ini, lakukan langkah-langkah berikut:**
  
 1. Memungkinkan semua orang untuk melihat anggota grup SharePoint.
  
 2. Menghapus Grup SharePoint dari kepada atau CC baris email.
  
 3. Secara eksplisit menambahkan pengguna ke kepada atau CC baris jika visibilitas keanggotaan tidak dapat diubah untuk grup SharePoint.
  
Untuk melihat rincian lebih lanjut silakan lihat [HTTP tidak sah untuk /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  