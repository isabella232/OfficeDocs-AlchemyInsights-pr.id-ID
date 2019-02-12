---
title: Sinkronisasi UPN dinonaktifkan
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 983796ce8fb7e8b52c0ce31aa13597b53cc9e038
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/12/2019
ms.locfileid: "29921711"
---
# <a name="upn-sync-disabled"></a>Sinkronisasi UPN dinonaktifkan

Jika Anda memulai sinkronisasi Azure iklan sebelum 30 Maret 2016, Jalankan cmdlet Azure iklan PowerShell berikut untuk mengaktifkan UPN lembut cocok untuk organisasi Anda hanya:
  
 **Set-MsolDirSyncFeature-fitur EnableSoftMatchOnUpn-mengaktifkan $True**
  
UPN lembut pertandingan secara otomatis diaktifkan untuk organisasi yang mulai sinkronisasi Azure iklan pada atau setelah tanggal 30 Maret 2016.
  
Untuk mempelajari lebih lanjut tentang mengaktifkan lembut cocok pada UPN dan fitur sinkronisasi lainnya, silakan lihat [Azure iklan menyambung sinkronisasi Layanan fitur](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

