---
title: Menggunakan PowerShell untuk berbagi kebijakan dan relasi organisasi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 717cdd6827e243ac6bf375209a911937c97088d2
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862089"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>Menggunakan PowerShell untuk berbagi kebijakan dan relasi organisasi


Untuk hubungan organisasi silakan Tinjau informasi rinci sintaks dan parameter untuk: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) dan [Hapus-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Untuk membuat kebijakan berbagi menggunakan [baru-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). Untuk [menerapkan kebijakan berbagi ke kotak pesan atau pengguna](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) , Anda harus menggunakan kombinasi [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) dan [Get-kotak surat](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) dengan kebijakan yang baru dibuat. Untuk [mengubah, menonaktifkan atau menghapus kebijakan berbagi](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) Anda perlu menggunakan [set-sharingpolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) dan [Hapus-sharingpolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**Untuk pemahaman penuh tentang topik ini silahkan baca:**

[Berbagi di Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing)