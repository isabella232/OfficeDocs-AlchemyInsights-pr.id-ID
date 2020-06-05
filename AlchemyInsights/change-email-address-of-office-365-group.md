---
title: Ubah Alamat email dari Microsoft 365 grup
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580660"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Ubah Alamat email dari Microsoft 365 grup

Anda dapat mengubah alamat email dari Microsoft 365 grup dengan menggunakan pusat admin. Cukup pilih grup dan pilih @edit alamat email.

Anda juga dapat menggunakan perintah EXO PowerShell untuk mengubah alamat SMTP primer Microsoft 365 grup:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress<new SMTP Address>

Contoh:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
