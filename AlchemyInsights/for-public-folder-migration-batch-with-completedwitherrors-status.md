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
ms.openlocfilehash: 4243cdf0170fed1eadac6560d2a04e1a861c63e5
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/15/2020
ms.locfileid: "42043595"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Untuk folder publik migrasi batch dengan status CompletedWithErrors

Gunakan langkah berikut untuk menyelesaikan batch, melewatkan item besar/buruk: 
1. Setujui item yang dilewati pada kumpulan migrasi:

    Set-MigrationBatch \<batchname>-ApproveSkippedItems 
2. Gunakan perintah berikut untuk menyetujui item yang dilewati pada permintaan migrasi yang "disinkronkan" namun tidak selesai:

    $pf = Dapatkan-PublicFolderMailboxMigrationRequest | Dapatkan-PublicFolderMailboxMigrationRequestStatistics-IncludeReport; ForEach ($i dalam $pf) {if ($i. LargeItemsEncountered-gt 0-atau $i. BadItemsEncountered-gt 0) {set-PublicFolderMailboxMigrationRequest $i. Identity. IdentifyingGuid-SkippedItemApprovalTime $ ([DateTime]:: UtcNow)}}
3. Kumpulan migrasi dan permintaan harus dilanjutkan dan diselesaikan dalam beberapa menit.

