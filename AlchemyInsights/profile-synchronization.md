---
title: Sinkronisasi profil
ms.author: arnek
author: arnek
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: dc6e0280961d14aa3e6bd466afbe0cbe89418d17
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43768116"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Kapan perubahan profil saya disinkronkan ke aplikasi profil pengguna SharePoint?

SharePoint Online menggunakan pekerjaan timer impor direktori aktif (AD impor) untuk mengimpor pengguna dan grup ke profil pengguna aplikasi. 
  
1. Impor AD Sync perubahan dari SharePoint online direktori penyimpanan ke profil pengguna aplikasi. Perubahan ini diproses dalam batch.
    
2. Pekerjaan timer berjalan hingga perubahan disinkronkan.
    
> [!NOTE]
> Waktu yang dibutuhkan untuk menjalankan pekerjaan tergantung pada jumlah perubahan proses. Sejumlah besar perubahan membutuhkan waktu lebih lama. Layanan tingkat perjanjian (SLA) menyatakan bahwa perubahan ke pengguna di direktori SharePoint online akan tercermin dalam aplikasi profil pengguna dalam 24 jam. 
  
[Info lebih lanjut tentang sinkronisasi profil pengguna di SharePoint online](https://go.microsoft.com/fwlink/?linkid=875671)
  

