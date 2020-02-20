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
ms.openlocfilehash: c4632b52dde579b7d5b2e6e15f1583300a0bd136
ms.sourcegitcommit: a7c17217c170ead24571421baaf5a14f1525b1a6
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/20/2020
ms.locfileid: "42157620"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Pensiun Legacy eDiscovery alat

Sebagai hasil dari fungsionalitas eDiscovery baru dan ditingkatkan di Microsoft 365 kepatuhan pusat, alat eDiscovery warisan berikut ini dan commandlets akan dihentikan dalam beberapa bulan mendatang:

- [EDiscovery di tempat](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) dan [pembekuan di tempat](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) di pusat admin Exchange.

- Cmdlet Exchange Online PowerShell yang mendukung eDiscovery di tempat dan pembekuan di tempat. (Cmdlet ini secara kolektif diidentifikasi sebagai *-MailboxSearch cmdlet.) Ini termasuk cmdlet berikut:

    - [Baru-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Mulai-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Cmdlet [pencarian-kotak surat](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) di Exchange Online PowerShell.
- Operasi berikut ini di Exchange Web Services API:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [Setholdonmailbox](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [Getholdonmailbox](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Office 365 lanjut eDiscovery v 1.0](https://docs.microsoft.com/en-us/microsoft-365/compliance/office-365-advanced-ediscovery)

**Timeline untuk pensiun**:
- 1 April 2020: Anda tidak akan dapat membuat penelusuran dan penangguhan baru, namun Anda masih dapat menjalankan, mengedit, dan menghapus penelusuran yang ada dengan risiko Anda sendiri. Dukungan Microsoft tidak lagi mendukung eDiscovery di tempat & pembekuan dalam EAC.

- 1 Juli 2020: eDiscovery di tempat & memegang fungsionalitas di EAC akan ditempatkan dalam mode baca-saja. Artinya, Anda hanya dapat menghapus penelusuran dan penangguhan yang ada.

**Untuk informasi lebih lanjut, lihat**:

 - [Migrasi pencarian eDiscovery warisan dan memegang pusat kepatuhan Microsoft 365](https://docs.microsoft.com/en-us/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Pensiun alat eDiscovery warisan](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Pertanyaan umum tentang eDiscovery di tempat dan pembekuan di tempat](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



