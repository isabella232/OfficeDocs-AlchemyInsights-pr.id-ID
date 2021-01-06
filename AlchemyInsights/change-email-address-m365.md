---
title: Mengubah alamat email grup Microsoft 365 atau Microsoft Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756560"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Mengubah alamat email grup Microsoft 365 atau Microsoft Teams

Anda dapat mengubah alamat email grup Microsoft 365 atau Microsoft Teams menggunakan [pusat admin Microsoft 365](https://admin.microsoft.com/). Cukup pilih grup lalu pilih @edit alamat email.

Anda juga dapat menggunakan perintah EXO PowerShell berikut untuk mengubah alamat SMTP utama grup Microsoft 365/Teams:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Contoh:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
