---
title: 2419-unable-to-enable-auditing
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 0566a8d002b1bd9e38f3184824193394e49d56494d347338f96cfcdfdb758f4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007793"
---
# <a name="unable-to-enable-unified-auditing"></a>Tidak dapat mengaktifkan pengauditan terpadu

Saat mencoba mengaktifkan pengauditan terpadu untuk organisasi, Anda mungkin menerima pesan kesalahan seperti berikut:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Untuk mengatasi masalah ini, ikuti langkah-langkah berikut:

1. [Koneksi ke Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Jalankan cmdlet berikut:

   ```
   Enable-OrganizationCustomization
   ```

3. Tunggu 60 menit hingga pengaturan sebelumnya diterapkan.

4. Jalankan perintah berikut ini di Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Untuk informasi tambahan, lihat artikel berikut ini:

- [Koneksi untuk Exchange Online PowerShell menggunakan multi-factor authentication](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Mengaktifkan atau menonaktifkan pencarian log audit](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
