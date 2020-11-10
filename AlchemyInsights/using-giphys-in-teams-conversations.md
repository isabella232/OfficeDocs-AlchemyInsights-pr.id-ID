---
title: Menggunakan Gipai dalam percakapan teams
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982506"
---
# <a name="using-giphys-in-teams-conversations"></a>Menggunakan Gipai dalam percakapan teams

Akses giphys di obrolan teams diaktifkan secara default. Sebagai administrator, Anda bisa mengontrol jika Giphys tersedia untuk pengguna dengan [mengatur kebijakan pesan](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) dan memastikan bahwa **gunakan giphys dalam percakapan** **aktif**.

Jika GIF tidak berfungsi seperti yang diharapkan dalam percakapan teams, verifikasi:

[Kebijakan pesan](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) perlu memperbolehkan Giphys. Untuk memverifikasi menggunakan cmdlet PowerShell:

- Verifikasi bahwa Anda bisa [mengelola teams dengan PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Jalankan perintah PowerShell [Get-CsTeamsMessagingPolicy-identitas global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) dan verifikasi bahwa **Allowgiphy** diatur ke **True**.
- Jika **Allowgiphy** diatur ke **false** , jalankan perintah PowerShell berikut ini [set-CsTeamsMessagingPolicy-identitas Global-allowgiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[Pengalaman terhubung opsional](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) perlu diaktifkan untuk memperbolehkan akses ke URL giphy.

> [!NOTE]
> Jika Anda memiliki beberapa tim pesan yang dikonfigurasi untuk penyewa Anda, Anda bisa menentukan identitas kebijakan yang ditetapkan untuk pengguna yang terkena dampak dengan perintah PowerShell [Get-CsOnlineUser-identitas](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Pilih TeamsMessagingPolicy.
