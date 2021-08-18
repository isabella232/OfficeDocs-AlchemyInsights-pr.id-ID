---
title: Menggunakan Giphy di Teams Percakapan
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
ms.openlocfilehash: 296c2f80d35f1c93ab3c60e0be65fd96c953ca81
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323523"
---
# <a name="using-giphys-in-teams-conversations"></a>Menggunakan Giphy di Teams Percakapan

Akses Giphy dalam Teams obrolan otomatis diaktifkan secara default. Sebagai administrator, Anda dapat mengontrol apakah Giphy [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) tersedia bagi pengguna dengan mengatur kebijakan olahpesan dan memastikan bahwa Gunakan **Giphy dalam percakapan** **aktif**.

Jika GIF tidak berfungsi seperti yang diharapkan Teams percakapan, verifikasi:

Kebijakan [pesan harus](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) memperbolehkan Giphys. Untuk memverifikasi menggunakan cmdlet PowerShell:

- Verifikasi bahwa Anda bisa [Mengelola Teams dengan PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Jalankan perintah PowerShell [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) dan pastikan bahwa **AllowGiphy** diatur ke **TRUE.**
- Jika **AllowGiphy** diatur ke **FALSE,** jalankan perintah PowerShell [berikut, Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[Pengalaman Terhubung Opsional](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) harus diaktifkan agar dapat mengakses URL Giphy.

**Catatan**: Jika Anda memiliki beberapa Teams Pesan yang dikonfigurasi untuk penyewa, Anda bisa menentukan identitas kebijakan yang ditetapkan untuk pengguna yang terkena dampak dengan perintah [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Pilih TeamsMessagingPolicy.
