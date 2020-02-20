---
title: Untuk folder publik migrasi batch dengan status CompletedWithErrors
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
- "3532"
ms.openlocfilehash: 739e9d91f90e4c0374814d199e4372eb5625553a
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158612"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Untuk folder publik migrasi batch dengan status CompletedWithErrors

Gunakan langkah berikut untuk menyelesaikan batch, melewatkan item besar/buruk: 
1. Setujui item yang dilewati pada kumpulan migrasi:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Gunakan perintah berikut untuk menyetujui item yang dilewati pada permintaan migrasi yang "disinkronkan" namun tidak selesai:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Kumpulan migrasi dan permintaan harus dilanjutkan dan diselesaikan dalam beberapa menit.

