---
title: Sinkronisasi UPN dinonaktifkan
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 33bc7e30d41ff70e2ce55d946202acf45dbcb0f2
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726107"
---
# <a name="upn-sync-disabled"></a>Sinkronisasi UPN dinonaktifkan

Jika Anda mulai menyinkronkan ke Azure AD sebelum 30 Maret 2016, jalankan berikut Azure AD PowerShell cmdlet untuk mengaktifkan UPN lembut cocok untuk organisasi Anda hanya:
  
 **Set-MsolDirSyncFeature-fitur EnableSoftMatchOnUpn-Enable $True**
  
Kecocokan lembut UPN secara otomatis diaktifkan untuk organisasi yang mulai menyinkronkan ke Azure AD pada atau setelah 30 Maret 2016.
  
Untuk mempelajari selengkapnya tentang mengaktifkan pencocokan lembut UPN dan fitur sinkronisasi lainnya, silakan lihat [AZURE AD menyambung sinkronisasi fitur layanan](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

