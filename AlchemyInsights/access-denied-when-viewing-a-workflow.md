---
title: Access denied when viewing a Workflow
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 2b076ec5dca070555ce51b88631fb6bd619ed9269e59ccc799b23b8b95547c16
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955204"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Access denied when viewing a Workflow

SharePoint Alur Kerja 2013 yang berusaha mengirim email ke grup SharePoint bisa gagal dengan pesan kesalahan "Akses Ditolak" jika keanggotaan grup SharePoint tidak diatur ke Semua Orang.
  
 **Untuk mengatasi masalah ini, lakukan langkah-langkah ini:**
  
 1. Memperbolehkan semua orang melihat anggota SharePoint grup.
  
 2. Hapus SharePoint grup dari baris Kepada atau CC email.
  
 3. Secara eksplisit menambahkan pengguna ke baris Kepada atau CC jika visibilitas keanggotaan tidak dapat diubah untuk SharePoint grup.
  
Untuk melihat detail selengkapnya, lihat HTTP Tidak Sah ke [/_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  