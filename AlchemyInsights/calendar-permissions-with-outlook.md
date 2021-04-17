---
title: Izin Kalender
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: bbd49134bd4a4451649b76bb5f60b19065910cae
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819911"
---
# <a name="calendar-permissions"></a>Izin Kalender

Pengguna dapat mengubah Izin Kalender mereka sendiri dengan Outlook di Web atau klien lain, tetapi sebagai admin Anda mungkin juga perlu menyelidikinya.  
Dengan cmdlet PowerShell Exchange akan memperlihatkan izin pada kalender pengguna:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Untuk melihat informasi selengkapnya, lihat yang berikut ini:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Izin Kalender digunakan dalam berbagi kalender, untuk melihat informasi selengkapnya tentang berbagi kalender Outlook, lihat artikel berikut ini:

- [Berbagi kalender Outlook dengan orang lain](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Berbagi kalender dalam Outlook di web untuk bisnis](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Untuk memecahkan masalah Izin Kalender, Anda dapat [menggunakan alat Asisten Dukungan dan](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) Pemulihan.