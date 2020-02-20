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
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="17398-102">Untuk folder publik migrasi batch dengan status CompletedWithErrors</span><span class="sxs-lookup"><span data-stu-id="17398-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="17398-103">Gunakan langkah berikut untuk menyelesaikan batch, melewatkan item besar/buruk:</span><span class="sxs-lookup"><span data-stu-id="17398-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="17398-104">Setujui item yang dilewati pada kumpulan migrasi:</span><span class="sxs-lookup"><span data-stu-id="17398-104">Approve the skipped items on migration batch:</span></span>

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. <span data-ttu-id="17398-105">Gunakan perintah berikut untuk menyetujui item yang dilewati pada permintaan migrasi yang "disinkronkan" namun tidak selesai:</span><span class="sxs-lookup"><span data-stu-id="17398-105">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. <span data-ttu-id="17398-106">Kumpulan migrasi dan permintaan harus dilanjutkan dan diselesaikan dalam beberapa menit.</span><span class="sxs-lookup"><span data-stu-id="17398-106">The migration batch and requests should resume and complete in a few minutes.</span></span>

