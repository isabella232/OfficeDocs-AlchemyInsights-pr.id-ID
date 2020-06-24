---
title: Izin kalender
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862092"
---
# <a name="calendar-permissions"></a>Izin kalender

Pengguna dapat mengubah izin kalender mereka sendiri dengan Outlook di web atau klien lain, tetapi sebagai admin Anda mungkin perlu untuk menyelidiki juga.  
Dengan cmdlet Exchange PowerShell akan menunjukkan izin pada kalender pengguna:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Untuk melihat informasi lebih lanjut, lihat hal berikut:

- [Dapatkan-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Tambah-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Izin kalender digunakan dalam berbagi kalender, untuk melihat informasi lebih lanjut tentang berbagi kalender Outlook, lihat artikel berikut:

- [Berbagi kalender Outlook dengan orang lain](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Berbagi kalender di Outlook di web untuk bisnis](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Untuk memecahkan masalah izin kalender Anda dapat menggunakan [dukungan dan alat asisten pemulihan](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) .