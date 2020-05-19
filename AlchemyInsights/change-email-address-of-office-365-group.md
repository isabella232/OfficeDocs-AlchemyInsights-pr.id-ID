---
title: Mengubah alamat email dari Microsoft 365 grup
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
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/27/2020
ms.locfileid: "44282926"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a>Mengubah alamat email dari Microsoft 365 grup

Anda dapat mengubah alamat email dari Microsoft 365 grup dengan menggunakan pusat admin. Cukup pilih grup dan pilih @edit alamat email.

Anda juga dapat menggunakan perintah EXO PowerShell untuk mengubah alamat SMTP primer Microsoft 365 grup:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress<new SMTP Address>

Contoh:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
