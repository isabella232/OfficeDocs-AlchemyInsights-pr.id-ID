---
title: 2419-tidak dapat diaktifkan-pengauditan
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
ms.openlocfilehash: 81fd8e33feb2f2b10b04cc7cdc746a8603aa366b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767602"
---
# <a name="unable-to-enable-unified-auditing"></a>Tidak dapat mengaktifkan pengauditan terpadu

Ketika Anda mencoba mengaktifkan pengauditan terpadu untuk organisasi, Anda mungkin menerima kesalahan yang sama seperti berikut ini:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Untuk mengatasi masalah ini, ikuti langkah-langkah berikut:

1. [Menyambungkan ke Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Jalankan cmdlet berikut:

   ```
   Enable-OrganizationCustomization
   ```

3. Tunggu hingga 60 menit agar pengaturan sebelumnya diterapkan.

4. Jalankan perintah berikut ini di Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Untuk informasi tambahan, lihat artikel berikut ini:

- [Menyambungkan ke Exchange Online PowerShell menggunakan autentikasi multifaktor](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Mengaktifkan atau menonaktifkan pencarian log audit](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
