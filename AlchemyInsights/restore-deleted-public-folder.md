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
ms.openlocfilehash: 7b04612daca61650d162c1dde240e25c1b185b04
ms.sourcegitcommit: 8ba12eff67e405f5922ea4cc35155e3036447859
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/15/2020
ms.locfileid: "42063676"
---
# <a name="restore-a-deleted-public-folder"></a>Memulihkan folder publik yang dihapus

**Untuk memulihkan item yang dihapus dari folder publik**:

- Lihat [Anda tidak dapat memulihkan item yang dihapus dari folder publik non-email di Outlook 2016](https://aka.ms/pfrec).
 
**Untuk memulihkan folder publik yang dihapus (dari jenis apa pun)**: 

- Silakan gunakan perintah EXO PowerShell berikut ini:

    Sintaks:

    >$pf = Get-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-Recurse |? {$_. Nama-EQ "\<name_of_deleted_public_Folder"}; Set-PublicFolder $pf. Identity-path \<path di mana folder akan dipulihkan>

    Contoh: perintah berikut akan mengembalikan Subfolder1 dan menempatkannya di bawah \Parent1:

    >$pf = Get-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-Recurse |? {$_. Nama-EQ "Subfolder1"}; Set-PublicFolder $pf. Identity-path \Parent1

Lihat [memulihkan folder publik yang dihapus](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) untuk rincian lebih lanjut.
