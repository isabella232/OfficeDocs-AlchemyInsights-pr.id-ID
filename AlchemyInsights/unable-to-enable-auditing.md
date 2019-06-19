---
title: 2419-tidak-untuk-Aktifkan-audit
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 3af01c03711eed646f0009afb5bea685bc358196
ms.sourcegitcommit: 87153fec6f6468b57893abf4aac073ba4068e67b
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/19/2019
ms.locfileid: "35065657"
---
# <a name="unable-to-enable-unified-auditing"></a>Mampu mengaktifkan audit bersatu

Ketika Anda mencoba untuk mengaktifkan audit bersatu untuk organisasi Office 365, Anda menerima galat yang mirip berikut:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Untuk mengatasi masalah ini, ikuti langkah berikut:

1. [Tersambung ke Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Jalankan cmdlet berikut:

   ```
   Enable-OrganizationCustomization
   ```

3. Tunggu selama 60 menit untuk pengaturan sebelumnya untuk diterapkan.

4. Jalankan perintah berikut dalam Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Untuk informasi tambahan, lihat artikel berikut:

- [Tersambung ke Exchange Online PowerShell menggunakan multi faktor otentikasi](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Mengaktifkan Office 365 audit log pencarian atau menonaktifkan](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
