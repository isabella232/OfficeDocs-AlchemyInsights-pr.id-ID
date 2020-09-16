---
title: Pensiun alat eDiscovery lawas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 2315c4c651a83f0ecc78c0171f32aba13bc93f8c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727786"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Pensiun alat eDiscovery lawas

Sebagai hasil dari fungsionalitas eDiscovery yang baru dan disempurnakan di pusat kepatuhan Microsoft 365, alat dan commandlet eDiscovery berikut ini akan dihentikan dalam bulan yang akan datang:

- [EDiscovery di tempat](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) dan [penangguhan di tempat](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) di pusat admin Exchange.

- Cmdlet PowerShell Exchange Online yang mendukung eDiscovery di tempat dan penangguhan di tempat. (Cmdlet ini secara keseluruhan diidentifikasi sebagai cmdlet *-MailboxSearch.) Ini termasuk cmdlet berikut:

    - [MailboxSearch baru](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Mulai-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Hentikan MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Cmdlet [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) di Exchange Online PowerShell.
- Operasi berikut ini di API Layanan web Exchange:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [Setholdonmailbox](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [Getholdonmailbox](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [V 1.0 eDiscovery tingkat lanjut](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Garis waktu untuk pensiun**:
- **1 juli 2020** Anda tidak lagi dapat membuat pencarian dan penangguhan baru, tapi Anda bisa menjalankan, mengedit, dan menghapus pencarian yang sudah ada dengan risiko Anda sendiri. Dukungan Microsoft tidak lagi mendukung penangguhan & tempat eDiscovery di EAC.
    
- **1 oktober 2020** & eDiscovery di tempat yang memegang fungsi di EAC akan ditempatkan dalam mode baca-saja, jadi Anda hanya dapat menghapus pencarian dan penangguhan yang sudah ada.

**Untuk informasi selengkapnya, lihat**:

 - [Melakukan migrasi pencarian eDiscovery warisan dan pembekuan ke pusat kepatuhan Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Pensiun alat eDiscovery lawas](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Tanya jawab umum tentang eDiscovery di tempat dan penangguhan di tempat](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



