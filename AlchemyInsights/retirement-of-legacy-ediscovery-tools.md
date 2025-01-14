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
ms.openlocfilehash: 2e7f898ac1a9e9469f633192be18e2a3a362023c83c9e510593196b5a4a0daf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074677"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Pensiun dari Alat eDiscovery Warisan

Sebagai hasil dari fungsi eDiscovery yang baru dan ditingkatkan di pusat Kepatuhan Microsoft 365, alat dan commandlet eDiscovery warisan berikut ini akan dihentikan dalam bulan-bulan mendatang:

- [In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) [and In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.

- Cmdlet PowerShell Exchange Online yang mendukung In-Place eDiscovery dan In-Place Pencarian. (Cmdlets ini secara kolektif diidentifikasi sebagai cmdlet *-MailboxSearch.) Hal ini mencakup cmdlet berikut:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Cmdlet [Cari-Kotak Surat](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) di Exchange Online PowerShell.
- Operasi berikut ini di Exchange API Layanan Web:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Garis waktu untuk pensiun:**
- **1 Juli 2020** Anda tidak lagi bisa membuat pencarian dan menahan, tapi Anda bisa menjalankan, mengedit, dan menghapus pencarian yang sudah ada dengan risiko Anda sendiri. Dukungan Microsoft tidak lagi In-Place dengan & eDiscovery di EAC.
    
- **1 Oktober 2020** In-Place fungsionalitas eDiscovery & Holds dalam EAC akan diletakkan dalam mode baca-saja, sehingga Anda hanya dapat menghapus pencarian dan menahan yang sudah ada.

**Untuk informasi selengkapnya, lihat:**

 - [Melakukan migrasi pencarian dan tahan eDiscovery warisan pada pusat kepatuhan Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Pensiun dari alat eDiscovery warisan](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Tanya Jawab Umum tentang In-Place eDiscovery dan In-Place Rapat](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



