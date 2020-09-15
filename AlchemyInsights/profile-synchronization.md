---
title: Sinkronisasi profil
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: eee1080a95955332e205db3852381e39aaf5ae0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801772"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Kapan profil saya berubah sinkronisasi ke aplikasi profil pengguna SharePoint?

SharePoint Online menggunakan pekerjaan timer impor direktori aktif (impor iklan) untuk mengimpor pengguna dan grup ke dalam aplikasi profil pengguna. 
  
1. Impor AD menyinkronkan perubahan dari Bursa direktori SharePoint online ke aplikasi profil pengguna. Perubahan ini diproses dalam batch.
    
2. Pekerjaan timer berjalan hingga perubahan disinkronkan.
    
> [!NOTE]
> Waktu yang diperlukan pekerjaan yang dijalankan bergantung pada jumlah perubahan yang akan diproses. Sejumlah besar perubahan memakan waktu lebih lama. Perjanjian tingkat layanan (SLA) menyatakan bahwa perubahan kepada pengguna di direktori SharePoint online akan tercermin dalam aplikasi profil pengguna dalam 24 jam. 
  
[Informasi selengkapnya tentang sinkronisasi profil pengguna di SharePoint online](https://go.microsoft.com/fwlink/?linkid=875671)
  

