---
title: 2419-tidak dapat-untuk-mengaktifkan-audit
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 23ad07a6dd943d61d1bd45453089a771cfd51b58
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510431"
---
# <a name="unable-to-enable-unified-auditing"></a>Tidak dapat mengaktifkan audit terpadu

Ketika Anda mencoba untuk mengaktifkan audit terpadu untuk organisasi Anda, Anda mungkin menerima galat yang serupa berikut ini:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Untuk mengatasi masalah ini, ikuti langkah berikut:

1. [Menyambung ke Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Jalankan cmdlet berikut:

   ```
   Enable-OrganizationCustomization
   ```

3. Tunggu 60 menit untuk pengaturan sebelumnya diterapkan.

4. Jalankan perintah berikut ini di Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Untuk informasi tambahan, lihat artikel berikut ini:

- [Menyambung ke Exchange Online PowerShell menggunakan otentikasi multi faktor](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Mengaktifkan atau menonaktifkan penelusuran log audit](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
