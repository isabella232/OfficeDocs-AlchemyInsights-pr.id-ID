---
title: Pensiun alat eDiscovery lawas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 94cd2127240be5faacd397ba6255fdb16e364308
ms.sourcegitcommit: d4fc2a03af69e28e96075812d040fdd34d2e23f0
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/26/2020
ms.locfileid: "46902623"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="79851-102">Pensiun alat eDiscovery lawas</span><span class="sxs-lookup"><span data-stu-id="79851-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="79851-103">Sebagai hasil dari fungsionalitas eDiscovery yang baru dan disempurnakan di pusat kepatuhan Microsoft 365, alat dan commandlet eDiscovery berikut ini akan dihentikan dalam bulan yang akan datang:</span><span class="sxs-lookup"><span data-stu-id="79851-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="79851-104">[EDiscovery di tempat](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) dan [penangguhan di tempat](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) di pusat admin Exchange.</span><span class="sxs-lookup"><span data-stu-id="79851-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="79851-105">Cmdlet PowerShell Exchange Online yang mendukung eDiscovery di tempat dan penangguhan di tempat.</span><span class="sxs-lookup"><span data-stu-id="79851-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="79851-106">(Cmdlet ini secara keseluruhan diidentifikasi sebagai cmdlet \*-MailboxSearch.) Ini termasuk cmdlet berikut:</span><span class="sxs-lookup"><span data-stu-id="79851-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="79851-107">MailboxSearch baru</span><span class="sxs-lookup"><span data-stu-id="79851-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="79851-108">Mulai-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="79851-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="79851-109">Hentikan MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="79851-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="79851-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="79851-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="79851-111">Cmdlet [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) di Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="79851-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="79851-112">Operasi berikut ini di API Layanan web Exchange:</span><span class="sxs-lookup"><span data-stu-id="79851-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="79851-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="79851-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="79851-114">Setholdonmailbox</span><span class="sxs-lookup"><span data-stu-id="79851-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="79851-115">Getholdonmailbox</span><span class="sxs-lookup"><span data-stu-id="79851-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="79851-116">V 1.0 eDiscovery tingkat lanjut</span><span class="sxs-lookup"><span data-stu-id="79851-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="79851-117">**Garis waktu untuk pensiun**:</span><span class="sxs-lookup"><span data-stu-id="79851-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="79851-118">**1 juli 2020** Anda tidak lagi dapat membuat pencarian dan penangguhan baru, tapi Anda bisa menjalankan, mengedit, dan menghapus pencarian yang sudah ada dengan risiko Anda sendiri.</span><span class="sxs-lookup"><span data-stu-id="79851-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="79851-119">Dukungan Microsoft tidak lagi mendukung penangguhan & tempat eDiscovery di EAC.</span><span class="sxs-lookup"><span data-stu-id="79851-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="79851-120">**1 oktober 2020** & eDiscovery di tempat yang memegang fungsi di EAC akan ditempatkan dalam mode baca-saja, jadi Anda hanya dapat menghapus pencarian dan penangguhan yang sudah ada.</span><span class="sxs-lookup"><span data-stu-id="79851-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="79851-121">**Untuk informasi selengkapnya, lihat**:</span><span class="sxs-lookup"><span data-stu-id="79851-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="79851-122">Melakukan migrasi pencarian eDiscovery warisan dan pembekuan ke pusat kepatuhan Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="79851-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="79851-123">Pensiun alat eDiscovery lawas</span><span class="sxs-lookup"><span data-stu-id="79851-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="79851-124">Tanya jawab umum tentang eDiscovery di tempat dan penangguhan di tempat</span><span class="sxs-lookup"><span data-stu-id="79851-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



