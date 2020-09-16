---
title: Izin kalender
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: cfee520e26587c0a649c08084853c31232d027f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748796"
---
# <a name="calendar-permissions"></a>Izin kalender

Pengguna dapat mengubah izin kalender mereka sendiri dengan Outlook di web atau klien lainnya, namun sebagai admin, Anda mungkin juga perlu menyelidiki.  
Dengan cmdlet Exchange PowerShell, Anda akan diperlihatkan izin pada kalender pengguna:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Untuk melihat informasi selengkapnya, lihat yang berikut ini:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Tambahkan MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Izin kalender digunakan dalam berbagi kalender, untuk melihat informasi selengkapnya tentang berbagi kalender Outlook, lihat artikel berikut ini:

- [Berbagi kalender Outlook dengan orang lain](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Berbagi kalender Anda di Outlook di web untuk bisnis](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Untuk memecahkan masalah izin kalender, Anda dapat menggunakan alat [asisten dukungan dan pemulihan](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) .