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
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="6ea8e-102">Memulihkan folder publik yang dihapus</span><span class="sxs-lookup"><span data-stu-id="6ea8e-102">Restore a deleted public folder</span></span>

<span data-ttu-id="6ea8e-103">**Untuk memulihkan item yang dihapus dari folder publik**:</span><span class="sxs-lookup"><span data-stu-id="6ea8e-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="6ea8e-104">Lihat [Anda tidak bisa memulihkan item terhapus dari folder publik non-email di Outlook 2016](https://aka.ms/pfrec).</span><span class="sxs-lookup"><span data-stu-id="6ea8e-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="6ea8e-105">**Untuk memulihkan folder publik yang dihapus (dari tipe apa pun)**:</span><span class="sxs-lookup"><span data-stu-id="6ea8e-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="6ea8e-106">Silakan gunakan perintah EXO PowerShell berikut ini:</span><span class="sxs-lookup"><span data-stu-id="6ea8e-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="6ea8e-107">Pascal</span><span class="sxs-lookup"><span data-stu-id="6ea8e-107">Syntax:</span></span>

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    <span data-ttu-id="6ea8e-108">Contoh: perintah berikut akan memulihkan Subfolder1 dan menempatkannya di bawah \Parent1:</span><span class="sxs-lookup"><span data-stu-id="6ea8e-108">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

<span data-ttu-id="6ea8e-109">Lihat [memulihkan folder publik yang dihapus](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) untuk detail selengkapnya.</span><span class="sxs-lookup"><span data-stu-id="6ea8e-109">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
