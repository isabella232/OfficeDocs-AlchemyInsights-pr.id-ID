---
title: Mengubah Microsoft Edge dengan menggunakan variabel direktori data dan bukan di garis namapenggunaanonim
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "9003873"
- "6926"
ms.openlocfilehash: 5c40aa1d7f61fbd2842839a5839899af8ab439f2
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/09/2020
ms.locfileid: "49677993"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hardcoded-paths"></a>Mengubah Microsoft Edge dengan menggunakan variabel direktori data dan bukan di garis namapenggunaanonim

Misalnya, di Windows, untuk menyimpan data profil di bawah data aplikasi lokal pengguna dan bukan di lokasi default, atur kebijakan **Userdatadir** ke **$ {local_app_data} \Edge\Profile**. 

Untuk mempelajari selengkapnya, lihat [membuat variabel direktori data pengguna Microsoft Edge](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars).