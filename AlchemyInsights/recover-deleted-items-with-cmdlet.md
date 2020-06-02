---
title: Memulihkan item yang dihapus dengan cmdlet
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800008"
- "5718"
ms.openlocfilehash: 86744d92a44096991079d1da3bdf4e95e58c55b7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/26/2020
ms.locfileid: "44493170"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="6fce9-102">Memulihkan item yang dihapus dengan cmdlet</span><span class="sxs-lookup"><span data-stu-id="6fce9-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="6fce9-103">Gunakan cmdlet [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) untuk melihat item yang dihapus di kotak pesan.</span><span class="sxs-lookup"><span data-stu-id="6fce9-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="6fce9-104">Setelah Anda menemukan item yang dihapus, Anda menggunakan cmdlet [RecoverableItems pemulihan](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) untuk memulihkan mereka.</span><span class="sxs-lookup"><span data-stu-id="6fce9-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="6fce9-105">Lihat rincian lengkap di [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="6fce9-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="6fce9-106">Anda harus ditetapkan peran ekspor impor kotak surat sebelum Anda dapat menjalankan cmdlet ini.</span><span class="sxs-lookup"><span data-stu-id="6fce9-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="6fce9-107">Silakan lihat [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) untuk informasi lebih lanjut.</span><span class="sxs-lookup"><span data-stu-id="6fce9-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
