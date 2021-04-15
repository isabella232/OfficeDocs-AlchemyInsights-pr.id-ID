---
title: Sinkronisasi UPN dinonaktifkan
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 2b1ba772459091ce1a796884997fe2516d0407eb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782154"
---
# <a name="upn-sync-disabled"></a>Sinkronisasi UPN dinonaktifkan

Jika mulai menyinkronkan ke Azure AD sebelum 30 Maret 2016, jalankan cmdlet PowerShell Azure AD berikut ini untuk mengaktifkan kecocokan lunak UPN hanya untuk organisasi Anda:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
Kecocokan lunak UPN secara otomatis diaktifkan untuk organisasi yang mulai menyinkronkan ke Azure AD pada atau setelah 30 Maret 2016.
  
Untuk mempelajari selengkapnya tentang mengaktifkan soft match pada UPN dan fitur sinkronisasi lainnya, silakan lihat [Fitur layanan sinkronisasi Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

