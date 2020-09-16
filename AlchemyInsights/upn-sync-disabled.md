---
title: Sinkronisasi UPN dinonaktifkan
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749517"
---
# <a name="upn-sync-disabled"></a>Sinkronisasi UPN dinonaktifkan

Jika Anda mulai menyinkronkan ke Azure AD sebelum 30 Maret 2016, Jalankan cmdlet Azure AD PowerShell berikut ini untuk mengaktifkan UPN pencocokan lembut hanya untuk organisasi Anda:
  
 **Set-MsolDirSyncFeature-fitur EnableSoftMatchOnUpn-Aktifkan $True**
  
Pencocokan lembut UPN diaktifkan secara otomatis untuk organisasi yang mulai menyinkronkan ke Azure AD pada atau setelah 30 Maret 2016.
  
Untuk mempelajari selengkapnya tentang mengaktifkan kecocokan lembut di UPN dan fitur sinkronisasi lainnya, silakan lihat [fitur layanan sinkronisasi AZURE AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

