---
title: Mengubah Microsoft Edge dengan menggunakan variabel direktori data dan bukan jalur yang berkode keras
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8222"
- "9004596"
ms.openlocfilehash: 23ce69157c465c56d0fc5ada7c2c159e3192fd75
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035820"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a>Mengubah Microsoft Edge dengan menggunakan variabel direktori data dan bukan jalur yang berkode keras

Misalnya, di Windows, untuk menyimpan data profil di bawah data aplikasi lokal pengguna dan bukan di lokasi default, atur kebijakan *Userdatadir* ke **$ {local_app_data} \Edge\Profile**.

Untuk informasi selengkapnya, lihat [membuat variabel direktori data pengguna Microsoft Edge](https://docs.microsoft.com/deployedge/microsoft-edge-policies).