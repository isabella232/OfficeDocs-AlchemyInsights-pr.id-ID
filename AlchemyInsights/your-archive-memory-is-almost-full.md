---
title: Kotak surat arsip Anda hampir penuh
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974406"
---
# <a name="your-archive-mailbox-is-almost-full"></a><span data-ttu-id="f49fc-102">Kotak surat arsip Anda hampir penuh</span><span class="sxs-lookup"><span data-stu-id="f49fc-102">Your archive mailbox is almost full</span></span>

<span data-ttu-id="f49fc-103">Jika pengguna menerima peringatan; **Kotak surat arsip Anda hampir penuh**, atau Anda perlu memperbesar ukuran kotak surat arsip, berikut ini beberapa tips:</span><span class="sxs-lookup"><span data-stu-id="f49fc-103">If the user receives the warning; **Your archive mailbox is almost full**, or you need to increase the size of their archive mailbox, here are some tips:</span></span>

1. <span data-ttu-id="f49fc-104">Jika pengguna ditetapkan ke lisensi Exchange Online paket 1, Mutakhirkan ke **Exchange Online paket 2** untuk menambah ukuran dari 50 GB ke 100gb.</span><span class="sxs-lookup"><span data-stu-id="f49fc-104">If the user is assigned an Exchange Online Plan 1, upgrade to **Exchange Online Plan 2** license to increase the size from 50 GB to 100GB.</span></span>
1. <span data-ttu-id="f49fc-105">Jika pengguna sudah ditetapkan salah satu hal berikut ini: **Exchange Online paket 2** atau Exchange Online paket 1 dengan add-on pengarsipan Exchange Online, gunakan langkah-langkah di bawah ini untuk mengaktifkan pengarsipan otomatis:.</span><span class="sxs-lookup"><span data-stu-id="f49fc-105">If the user is already assigned either of the following: **Exchange Online Plan 2** or an Exchange Online Plan 1 with an Exchange Online Archiving add-on, use the steps below to enable Auto-Expanding archiving:.</span></span>
 
    1. <span data-ttu-id="f49fc-106">[Menyambungkan ke Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="f49fc-106">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span></span>
    2. <span data-ttu-id="f49fc-107">Jalankan unifiedgroup berikut ini untuk pengguna:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span><span class="sxs-lookup"><span data-stu-id="f49fc-107">Run the following commandlet for the user:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span></span>
    1. <span data-ttu-id="f49fc-108">Jalankan unifiedgroup berikut ini untuk mengonfirmasinya diaktifkan untuk pengguna:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span><span class="sxs-lookup"><span data-stu-id="f49fc-108">Run the following commandlet to confirm it is enabled for the user:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span></span>

<span data-ttu-id="f49fc-109">Untuk informasi selengkapnya, lihat:</span><span class="sxs-lookup"><span data-stu-id="f49fc-109">For more information see:</span></span>

- [<span data-ttu-id="f49fc-110"> Mengaktifkan pengarsipan tak terbatas-bantuan admin-kepatuhan Microsoft 365 | Dokumen Microsoft</span><span class="sxs-lookup"><span data-stu-id="f49fc-110"> Enable unlimited archiving - Admin Help - Microsoft 365 Compliance | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [<span data-ttu-id="f49fc-111">Batas-Deskripsi Layanan Exchange Online | Dokumen Microsoft</span><span class="sxs-lookup"><span data-stu-id="f49fc-111">Exchange Online limits - Service Descriptions | Microsoft Docs</span></span>](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [<span data-ttu-id="f49fc-112">Memutakhirkan ke paket bisnis yang berbeda | Dokumen Microsoft</span><span class="sxs-lookup"><span data-stu-id="f49fc-112">Upgrade to a different business plan | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

