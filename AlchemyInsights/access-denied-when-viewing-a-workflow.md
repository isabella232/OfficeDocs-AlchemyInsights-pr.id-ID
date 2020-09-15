---
title: Akses ditolak saat menampilkan alur kerja
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 710775e8b2dee98969df7a4c8410a3e61181aaf6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688805"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Akses ditolak saat menampilkan alur kerja

Alur kerja SharePoint 2013 yang mencoba mengirim email ke grup SharePoint bisa gagal dengan pesan kesalahan "Akses ditolak" Jika keanggotaan grup SharePoint tidak diatur ke semua orang.
  
 **Untuk mengatasi masalah ini, lakukan langkah-langkah ini:**
  
 1. Izinkan semua orang melihat anggota grup SharePoint.
  
 2. Hapus grup SharePoint dari baris kepada atau CC dari email.
  
 3. Menambahkan pengguna secara eksplisit ke baris kepada atau CC jika visibilitas keanggotaan tidak bisa diubah untuk grup SharePoint.
  
Untuk melihat detail selengkapnya, lihat [http tidak sah ke/_vti_bin/client.SVC/SP.Utilities.Utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  