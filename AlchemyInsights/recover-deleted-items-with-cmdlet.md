---
title: Memulihkan item yang dihapus dengan cmdlet
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800008"
- "5718"
ms.openlocfilehash: d8f2a50f39d7bcd321692ab093e2efa6613e9814
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835814"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="caa7a-102">Memulihkan item yang dihapus dengan cmdlet</span><span class="sxs-lookup"><span data-stu-id="caa7a-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="caa7a-103">Gunakan cmdlet [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) untuk menampilkan item yang dihapus dalam kotak surat.</span><span class="sxs-lookup"><span data-stu-id="caa7a-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="caa7a-104">Setelah menemukan item yang dihapus, gunakan cmdlet [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) untuk memulihkannya.</span><span class="sxs-lookup"><span data-stu-id="caa7a-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="caa7a-105">Lihat detail selengkapnya di [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="caa7a-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="caa7a-106">Anda harus mendapatkan peran Ekspor Impor Kotak Surat sebelum dapat menjalankan cmdlet ini.</span><span class="sxs-lookup"><span data-stu-id="caa7a-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="caa7a-107">Lihat [Get-RecoverableItem](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) untuk informasi selengkapnya.</span><span class="sxs-lookup"><span data-stu-id="caa7a-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
