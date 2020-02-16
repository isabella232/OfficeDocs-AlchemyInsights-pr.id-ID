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
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="0a947-102">Memulihkan folder publik yang dihapus</span><span class="sxs-lookup"><span data-stu-id="0a947-102">Restore a deleted public folder</span></span>

<span data-ttu-id="0a947-103">**Untuk memulihkan item yang dihapus dari folder publik**:</span><span class="sxs-lookup"><span data-stu-id="0a947-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="0a947-104">Lihat [Anda tidak dapat memulihkan item yang dihapus dari folder publik non-email di Outlook 2016](https://aka.ms/pfrec).</span><span class="sxs-lookup"><span data-stu-id="0a947-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="0a947-105">**Untuk memulihkan folder publik yang dihapus (dari jenis apa pun)**:</span><span class="sxs-lookup"><span data-stu-id="0a947-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="0a947-106">Silakan gunakan perintah EXO PowerShell berikut ini:</span><span class="sxs-lookup"><span data-stu-id="0a947-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="0a947-107">Sintaks:</span><span class="sxs-lookup"><span data-stu-id="0a947-107">Syntax:</span></span>

    ><span data-ttu-id="0a947-108">$pf = Get-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-Recurse |? {$_. Nama-EQ "\<name_of_deleted_public_Folder"}; Set-PublicFolder $pf. Identity-path \<path di mana folder akan dipulihkan></span><span class="sxs-lookup"><span data-stu-id="0a947-108">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored></span></span>

    <span data-ttu-id="0a947-109">Contoh: perintah berikut akan mengembalikan Subfolder1 dan menempatkannya di bawah \Parent1:</span><span class="sxs-lookup"><span data-stu-id="0a947-109">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    ><span data-ttu-id="0a947-110">$pf = Get-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-Recurse |? {$_. Nama-EQ "Subfolder1"}; Set-PublicFolder $pf. Identity-path \Parent1</span><span class="sxs-lookup"><span data-stu-id="0a947-110">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1</span></span>

<span data-ttu-id="0a947-111">Lihat [memulihkan folder publik yang dihapus](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) untuk rincian lebih lanjut.</span><span class="sxs-lookup"><span data-stu-id="0a947-111">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
