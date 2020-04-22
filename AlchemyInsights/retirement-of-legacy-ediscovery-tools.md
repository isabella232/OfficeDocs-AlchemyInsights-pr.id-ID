---
title: Pensiun Legacy eDiscovery alat
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
ms.openlocfilehash: 262cca0feee17d1f929a5a94a4dd6c1ec317f6ec
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/21/2020
ms.locfileid: "43650571"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="4492a-102">Pensiun Legacy eDiscovery alat</span><span class="sxs-lookup"><span data-stu-id="4492a-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="4492a-103">Sebagai hasil dari fungsionalitas eDiscovery baru dan ditingkatkan di Microsoft 365 kepatuhan pusat, alat eDiscovery warisan berikut ini dan commandlets akan dihentikan dalam beberapa bulan mendatang:</span><span class="sxs-lookup"><span data-stu-id="4492a-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="4492a-104">[EDiscovery di tempat](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) dan [pembekuan di tempat](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) di pusat admin Exchange.</span><span class="sxs-lookup"><span data-stu-id="4492a-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="4492a-105">Cmdlet Exchange Online PowerShell yang mendukung eDiscovery di tempat dan pembekuan di tempat.</span><span class="sxs-lookup"><span data-stu-id="4492a-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="4492a-106">(Cmdlet ini secara kolektif diidentifikasi sebagai \*-MailboxSearch cmdlet.) Ini termasuk cmdlet berikut:</span><span class="sxs-lookup"><span data-stu-id="4492a-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="4492a-107">Baru-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="4492a-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="4492a-108">Mulai-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="4492a-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="4492a-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="4492a-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="4492a-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="4492a-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="4492a-111">Cmdlet [pencarian-kotak surat](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) di Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="4492a-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="4492a-112">Operasi berikut ini di Exchange Web Services API:</span><span class="sxs-lookup"><span data-stu-id="4492a-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="4492a-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="4492a-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="4492a-114">Setholdonmailbox</span><span class="sxs-lookup"><span data-stu-id="4492a-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="4492a-115">Getholdonmailbox</span><span class="sxs-lookup"><span data-stu-id="4492a-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="4492a-116">Lanjut eDiscovery v 1.0</span><span class="sxs-lookup"><span data-stu-id="4492a-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="4492a-117">**Timeline untuk pensiun**:</span><span class="sxs-lookup"><span data-stu-id="4492a-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="4492a-118">1 April 2020: Anda tidak akan dapat membuat penelusuran dan penangguhan baru, namun Anda masih dapat menjalankan, mengedit, dan menghapus penelusuran yang ada dengan risiko Anda sendiri.</span><span class="sxs-lookup"><span data-stu-id="4492a-118">April 1, 2020: You won't be able to create new searches and holds, but you can still run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="4492a-119">Dukungan Microsoft tidak lagi mendukung eDiscovery di tempat & pembekuan dalam EAC.</span><span class="sxs-lookup"><span data-stu-id="4492a-119">Microsoft Support will no longer support In-Place eDiscovery & Holds in the EAC.</span></span>

- <span data-ttu-id="4492a-120">1 Juli 2020: eDiscovery di tempat & memegang fungsionalitas di EAC akan ditempatkan dalam mode baca-saja.</span><span class="sxs-lookup"><span data-stu-id="4492a-120">July 1, 2020: The In-Place eDiscovery & Holds functionality in the EAC will be placed in a read-only mode.</span></span> <span data-ttu-id="4492a-121">Artinya, Anda hanya dapat menghapus penelusuran dan penangguhan yang ada.</span><span class="sxs-lookup"><span data-stu-id="4492a-121">This means you'll only be able to remove existing searches and holds.</span></span>

<span data-ttu-id="4492a-122">**Untuk informasi lebih lanjut, lihat**:</span><span class="sxs-lookup"><span data-stu-id="4492a-122">**For more information, see**:</span></span>

 - [<span data-ttu-id="4492a-123">Migrasi pencarian eDiscovery warisan dan memegang pusat kepatuhan Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="4492a-123">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="4492a-124">Pensiun alat eDiscovery warisan</span><span class="sxs-lookup"><span data-stu-id="4492a-124">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="4492a-125">Pertanyaan umum tentang eDiscovery di tempat dan pembekuan di tempat</span><span class="sxs-lookup"><span data-stu-id="4492a-125">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



