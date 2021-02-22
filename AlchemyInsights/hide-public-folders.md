---
title: Menyembunyikan folder publik
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 70179296e9c1bb7391535f55796bc5af80b825f8
ms.sourcegitcommit: a019bd8b0244914edb59e124bc6538cdc5c158f9
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/18/2021
ms.locfileid: "50315373"
---
# <a name="hide-public-folders"></a>Menyembunyikan folder publik

**Untuk menyembunyikan seluruh pohon folder publik**:

Gunakan langkah-langkah dalam artikel [ini](https://aka.ms/ControlPF) untuk menyembunyikan seluruh pohon folder publik dari pengguna selektif atau semua.

**Untuk menyembunyikan folder publik tertentu**:

1. Menambahkan izin untuk pengguna yang perlu mengakses folder publik

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. Hapus pengguna **default** dari daftar **izin** :

    `Remove-PublicFolderClientPermission \test1 -User Default`
