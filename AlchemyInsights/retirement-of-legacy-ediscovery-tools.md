---
title: Pensiun dari Alat eDiscovery Warisan
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
- "9001487"
- "3523"
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798552"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="4e69e-102">Pensiun dari Alat eDiscovery Warisan</span><span class="sxs-lookup"><span data-stu-id="4e69e-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="4e69e-103">Sebagai hasil dari fungsi eDiscovery yang baru dan diperbaiki dalam pusat Kepatuhan Microsoft 365, alat dan commandlet eDiscovery warisan berikut ini akan dihentikan dalam beberapa bulan mendatang:</span><span class="sxs-lookup"><span data-stu-id="4e69e-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="4e69e-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) [and In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span><span class="sxs-lookup"><span data-stu-id="4e69e-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="4e69e-105">Cmdlet PowerShell Exchange Online yang mendukung In-Place eDiscovery dan In-Place Pencarian.</span><span class="sxs-lookup"><span data-stu-id="4e69e-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="4e69e-106">(Cmdlets ini secara kolektif diidentifikasi sebagai cmdlet \*-MailboxSearch.) Hal ini mencakup cmdlet berikut:</span><span class="sxs-lookup"><span data-stu-id="4e69e-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="4e69e-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="4e69e-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="4e69e-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="4e69e-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="4e69e-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="4e69e-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="4e69e-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="4e69e-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="4e69e-111">Cmdlet [Cari-Kotak Surat](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) di Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="4e69e-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="4e69e-112">Operasi berikut ini di API Layanan Web Exchange:</span><span class="sxs-lookup"><span data-stu-id="4e69e-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="4e69e-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="4e69e-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="4e69e-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="4e69e-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="4e69e-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="4e69e-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="4e69e-116">Advanced eDiscovery v1.0</span><span class="sxs-lookup"><span data-stu-id="4e69e-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="4e69e-117">**Garis waktu untuk pensiun:**</span><span class="sxs-lookup"><span data-stu-id="4e69e-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="4e69e-118">**1 Juli 2020** Anda tidak lagi bisa membuat pencarian dan menahan, tapi Anda bisa menjalankan, mengedit, dan menghapus pencarian yang sudah ada dengan risiko Anda sendiri.</span><span class="sxs-lookup"><span data-stu-id="4e69e-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="4e69e-119">Dukungan Microsoft tidak lagi In-Place dengan & eDiscovery di EAC.</span><span class="sxs-lookup"><span data-stu-id="4e69e-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="4e69e-120">**1 Oktober 2020** In-Place fungsionalitas eDiscovery & Holds dalam EAC akan diletakkan dalam mode baca-saja, sehingga Anda hanya dapat menghapus pencarian dan menahan yang sudah ada.</span><span class="sxs-lookup"><span data-stu-id="4e69e-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="4e69e-121">**Untuk informasi selengkapnya, lihat:**</span><span class="sxs-lookup"><span data-stu-id="4e69e-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="4e69e-122">Melakukan migrasi pencarian dan tahan eDiscovery warisan ke pusat kepatuhan Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="4e69e-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="4e69e-123">Pensiun dari alat eDiscovery warisan</span><span class="sxs-lookup"><span data-stu-id="4e69e-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="4e69e-124">Tanya Jawab Umum tentang In-Place eDiscovery dan In-Place Rapat</span><span class="sxs-lookup"><span data-stu-id="4e69e-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



