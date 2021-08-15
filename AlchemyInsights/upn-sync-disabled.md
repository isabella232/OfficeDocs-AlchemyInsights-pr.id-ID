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
ms.openlocfilehash: fc163fae4d348d7c7cf117bd457f999b42f96bec7c1eb9aa1435e346131d06de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038115"
---
# <a name="upn-sync-disabled"></a>Sinkronisasi UPN dinonaktifkan

Jika mulai menyinkronkan ke Azure AD sebelum 30 Maret 2016, jalankan cmdlet PowerShell Azure AD berikut ini untuk mengaktifkan kecocokan lunak UPN hanya untuk organisasi Anda:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
Kecocokan lunak UPN secara otomatis diaktifkan untuk organisasi yang mulai menyinkronkan ke Azure AD pada atau setelah 30 Maret 2016.
  
Untuk mempelajari selengkapnya tentang mengaktifkan kecocokan sementara di UPN dan fitur sinkronisasi lainnya, silakan lihat [Azure AD Koneksi fitur layanan sinkronisasi](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

