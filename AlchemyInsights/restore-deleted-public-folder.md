---
title: Memulihkan folder publik yang dihapus
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: d5480389c3bf50cee9fe30f7ec8d8ff28ef694ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809442"
---
# <a name="restore-a-deleted-public-folder"></a>Memulihkan folder publik yang dihapus

**Untuk memulihkan item terhapus dari folder publik:**

- Lihat [Anda tidak dapat memulihkan item terhapus dari folder publik non-email di Outlook 2016](https://aka.ms/pfrec).
 
**Untuk memulihkan folder publik yang dihapus (tipe apa pun)**: 

- Silakan gunakan perintah PowerShell EXO berikut ini:

    Sintaks:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Contoh: Perintah berikut akan memulihkan Subfolder1 dan menempatkannya di bawah \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Lihat [Memulihkan folder publik yang dihapus](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) untuk detail selengkapnya.
