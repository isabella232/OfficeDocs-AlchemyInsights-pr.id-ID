---
title: Sinkronisasi profil
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: d1a72a85767e36fefbfa8eee266befcaf2e48af0
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/23/2019
ms.locfileid: "32371987"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Kapan perubahan profil Saya sync ke SharePoint pengguna profil aplikasi?

SharePoint Online menggunakan Active Directory impor pekerjaan timer (AD Import) untuk mengimpor pengguna dan grup ke profil pengguna aplikasi. 
  
1. Iklan impor syncs perubahan dari SharePoint Online direktori toko aplikasi profil pengguna. Perubahan ini diproses dalam batch.
    
2. Pekerjaan timer berjalan sampai perubahan disinkronkan.
    
> [!NOTE]
> Waktu yang dibutuhkan untuk menjalankan pekerjaan tergantung pada jumlah perubahan untuk memproses. Sejumlah besar perubahan memakan waktu lama. Service Level Agreement (SLA) menyatakan bahwa perubahan ke pengguna dalam direktori Online SharePoint akan tercermin dalam profil pengguna aplikasi dalam 24 jam. 
  
[Info lebih lanjut tentang sinkronisasi profil pengguna di SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

