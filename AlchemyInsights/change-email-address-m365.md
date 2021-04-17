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
ms.openlocfilehash: 7800a447c5dfcc8397121e1149921916ff7944ac
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819083"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Mengubah alamat email grup Microsoft 365 atau Microsoft Teams

Anda dapat mengubah alamat email grup Microsoft 365 atau Microsoft Teams menggunakan [pusat admin Microsoft 365](https://admin.microsoft.com/). Cukup pilih grup lalu pilih @edit alamat email.

Anda juga dapat menggunakan perintah EXO PowerShell berikut untuk mengubah alamat SMTP utama grup Microsoft 365/Teams:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Contoh:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
