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
ms.openlocfilehash: 6df196fc0bde37c962e3aa84dd602ee414dad3d329addfd16cb6e3dcc40fc2ae
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53943378"
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
