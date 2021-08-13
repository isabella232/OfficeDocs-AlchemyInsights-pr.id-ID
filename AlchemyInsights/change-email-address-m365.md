---
title: Mengubah alamat email grup Microsoft 365 atau Microsoft Teams
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
- "1200024"
- "4704"
ms.openlocfilehash: acb343553bfb7e100c03d0e7046ed5cbdd6b739b9a61e3faf17768bd8aadff34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995625"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Mengubah alamat email grup Microsoft 365 atau Microsoft Teams

Anda dapat mengubah alamat email grup Microsoft 365 atau Microsoft Teams menggunakan [pusat admin Microsoft 365](https://admin.microsoft.com/). Cukup pilih grup lalu pilih @edit alamat email.

Anda juga dapat menggunakan perintah EXO PowerShell berikut untuk mengubah alamat SMTP utama grup Microsoft 365/Teams:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Contoh:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
