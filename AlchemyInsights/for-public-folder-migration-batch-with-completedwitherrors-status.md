---
title: Untuk kumpulan migrasi folder publik dengan status CompletedWithErrors
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
- "3532"
ms.openlocfilehash: cbf5237fdb5c660057465e67702e35f68e545ddb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744116"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Untuk kumpulan migrasi folder publik dengan status CompletedWithErrors

Gunakan langkah-langkah berikut ini untuk menyelesaikan kumpulan, melompati item besar/buruk: 
1. Setujui item yang dilewati pada kumpulan migrasi:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Gunakan perintah berikut untuk menyetujui item yang dilewati pada permintaan migrasi yang "disinkronkan" tapi tidak selesai:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Kumpulan migrasi dan permintaan harus dilanjutkan dan diselesaikan dalam beberapa menit.

