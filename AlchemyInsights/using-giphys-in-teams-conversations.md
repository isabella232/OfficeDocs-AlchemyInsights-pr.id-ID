---
title: Menggunakan Giphy di Teams Conversations
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
ms.openlocfilehash: 0244b68ffa2ebd3d70bae66a24ac299004848557b63b17c2ea74fafaff22bb8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104311"
---
# <a name="using-giphys-in-teams-conversations"></a>Menggunakan Giphy di Teams Conversations

Akses Giphys Teams obrolan diaktifkan secara default. Sebagai administrator, Anda dapat mengontrol apakah Giphy [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) tersedia bagi pengguna dengan mengatur kebijakan olahpesan dan memastikan bahwa Gunakan **Giphy dalam percakapan** **aktif**.

Jika GIF tidak berfungsi seperti yang diharapkan Teams percakapan, verifikasi:

Kebijakan [pesan harus](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) memperbolehkan Giphys. Untuk memverifikasi menggunakan cmdlet PowerShell:

- Verifikasi bahwa Anda bisa [Mengelola Teams dengan PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Jalankan perintah PowerShell [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) dan pastikan bahwa **AllowGiphy** diatur ke **TRUE.**
- Jika **AllowGiphy** diatur ke **FALSE,** jalankan perintah PowerShell [berikut, Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[Pengalaman Terhubung Opsional](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) harus diaktifkan agar dapat mengakses URL Giphy.

> [!NOTE]
> Jika memiliki beberapa Teams Pesan yang dikonfigurasi untuk penyewa, Anda dapat menentukan identitas kebijakan yang ditetapkan untuk pengguna yang terkena dampak dengan perintah [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Pilih TeamsMessagingPolicy.
