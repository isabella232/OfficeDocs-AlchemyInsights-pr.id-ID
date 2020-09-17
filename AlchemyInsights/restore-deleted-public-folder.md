---
title: Memulihkan folder publik yang dihapus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: bb7fe248714e9a7e7f4c48913b159b5c23132192
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774534"
---
# <a name="restore-a-deleted-public-folder"></a>Memulihkan folder publik yang dihapus

**Untuk memulihkan item yang dihapus dari folder publik**:

- Lihat [Anda tidak bisa memulihkan item terhapus dari folder publik non-email di Outlook 2016](https://aka.ms/pfrec).
 
**Untuk memulihkan folder publik yang dihapus (dari tipe apa pun)**: 

- Silakan gunakan perintah EXO PowerShell berikut ini:

    Pascal

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Contoh: perintah berikut akan memulihkan Subfolder1 dan menempatkannya di bawah \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Lihat [memulihkan folder publik yang dihapus](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) untuk detail selengkapnya.
