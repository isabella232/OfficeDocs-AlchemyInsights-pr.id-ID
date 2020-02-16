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
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="52949-102">Untuk folder publik migrasi batch dengan status CompletedWithErrors</span><span class="sxs-lookup"><span data-stu-id="52949-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="52949-103">Gunakan langkah berikut untuk menyelesaikan batch, melewatkan item besar/buruk:</span><span class="sxs-lookup"><span data-stu-id="52949-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="52949-104">Setujui item yang dilewati pada kumpulan migrasi:</span><span class="sxs-lookup"><span data-stu-id="52949-104">Approve the skipped items on migration batch:</span></span>

    <span data-ttu-id="52949-105">Set-MigrationBatch \<batchname>-ApproveSkippedItems</span><span class="sxs-lookup"><span data-stu-id="52949-105">Set-MigrationBatch \<batchname> -ApproveSkippedItems</span></span> 
2. <span data-ttu-id="52949-106">Gunakan perintah berikut untuk menyetujui item yang dilewati pada permintaan migrasi yang "disinkronkan" namun tidak selesai:</span><span class="sxs-lookup"><span data-stu-id="52949-106">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    <span data-ttu-id="52949-107">$pf = Dapatkan-PublicFolderMailboxMigrationRequest | Dapatkan-PublicFolderMailboxMigrationRequestStatistics-IncludeReport; ForEach ($i dalam $pf) {if ($i. LargeItemsEncountered-gt 0-atau $i. BadItemsEncountered-gt 0) {set-PublicFolderMailboxMigrationRequest $i. Identity. IdentifyingGuid-SkippedItemApprovalTime $ ([DateTime]:: UtcNow)}}</span><span class="sxs-lookup"><span data-stu-id="52949-107">$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}</span></span>
3. <span data-ttu-id="52949-108">Kumpulan migrasi dan permintaan harus dilanjutkan dan diselesaikan dalam beberapa menit.</span><span class="sxs-lookup"><span data-stu-id="52949-108">The migration batch and requests should resume and complete in a few minutes.</span></span>

