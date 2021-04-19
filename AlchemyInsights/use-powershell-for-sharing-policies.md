---
title: Menggunakan Windows PowerShell untuk kebijakan Berbagi dan hubungan Organisasi
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
- "3800014"
- "898"
ms.openlocfilehash: 9c52b876160f9577e6cefe7644c29d6fdf3b23fd
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826058"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>Menggunakan Windows PowerShell untuk kebijakan Berbagi dan hubungan Organisasi


Untuk hubungan Organisasi, tinjau detail informasi sintaksis dan parameter mendetail untuk: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  DAN  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Untuk membuat kebijakan berbagi, gunakan [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). Untuk  [menerapkan kebijakan berbagi ke kotak surat atau pengguna](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes),  Anda perlu menggunakan kombinasi  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) dan [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) dengan kebijakan yang baru dibuat. Untuk  [mengubah, menonaktifkan, atau menghapus kebijakan berbagi](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy),  Anda perlu menggunakan  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) dan [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**Untuk pemahaman menyeluruh tentang topik ini, silakan baca:**

[Berbagi di Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing)