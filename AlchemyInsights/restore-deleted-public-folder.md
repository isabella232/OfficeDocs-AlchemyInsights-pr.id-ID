---
title: Memulihkan folder publik yang dihapus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: cd85dd3c0eb14f6e02ac4f912e733468403387aa
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158508"
---
# <a name="restore-a-deleted-public-folder"></a>Memulihkan folder publik yang dihapus

**Untuk memulihkan item yang dihapus dari folder publik**:

- Lihat [Anda tidak dapat memulihkan item yang dihapus dari folder publik non-email di Outlook 2016](https://aka.ms/pfrec).
 
**Untuk memulihkan folder publik yang dihapus (dari jenis apa pun)**: 

- Silakan gunakan perintah EXO PowerShell berikut ini:

    Sintaks:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Contoh: perintah berikut akan mengembalikan Subfolder1 dan menempatkannya di bawah \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Lihat [memulihkan folder publik yang dihapus](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) untuk rincian lebih lanjut.
