---
title: Untuk kumpulan migrasi folder publik dengan status CompletedWithErrors
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
- "3532"
ms.openlocfilehash: 9ed21bfb9069b56a4fc59b201bb3ad94c6bb6712
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812467"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Untuk kumpulan migrasi folder publik dengan status CompletedWithErrors

Gunakan langkah-langkah berikut untuk menyelesaikan kumpulan, melewati item besar/buruk: 
1. Menyetujui item yang dilewati pada kumpulan migrasi:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Gunakan perintah berikut untuk menyetujui item yang dilewati dalam permintaan migrasi yang "Disinkronkan" tetapi belum selesai:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Kumpulan dan permintaan migrasi harus dilanjutkan dan diselesaikan dalam beberapa menit.

