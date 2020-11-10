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
# <a name="using-giphys-in-teams-conversations"></a><span data-ttu-id="c5750-102">Menggunakan Gipai dalam percakapan teams</span><span class="sxs-lookup"><span data-stu-id="c5750-102">Using Giphys in Teams Conversations</span></span>

<span data-ttu-id="c5750-103">Akses giphys di obrolan teams diaktifkan secara default.</span><span class="sxs-lookup"><span data-stu-id="c5750-103">Giphys access in Teams chat is enabled by default.</span></span> <span data-ttu-id="c5750-104">Sebagai administrator, Anda bisa mengontrol jika Giphys tersedia untuk pengguna dengan [mengatur kebijakan pesan](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) dan memastikan bahwa **gunakan giphys dalam percakapan** **aktif**.</span><span class="sxs-lookup"><span data-stu-id="c5750-104">As an administrator, you can control if Giphys are available to users by [setting a messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) and ensuring that **Use Giphys in conversations** is **On**.</span></span>

<span data-ttu-id="c5750-105">Jika GIF tidak berfungsi seperti yang diharapkan dalam percakapan teams, verifikasi:</span><span class="sxs-lookup"><span data-stu-id="c5750-105">If GIFs are not working as expected in Teams conversations, verify:</span></span>

<span data-ttu-id="c5750-106">[Kebijakan pesan](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) perlu memperbolehkan Giphys.</span><span class="sxs-lookup"><span data-stu-id="c5750-106">The [messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) needs to allow Giphys.</span></span> <span data-ttu-id="c5750-107">Untuk memverifikasi menggunakan cmdlet PowerShell:</span><span class="sxs-lookup"><span data-stu-id="c5750-107">To verify by using PowerShell cmdlets:</span></span>

- <span data-ttu-id="c5750-108">Verifikasi bahwa Anda bisa [mengelola teams dengan PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span><span class="sxs-lookup"><span data-stu-id="c5750-108">Verify that you can [Manage Teams with PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span></span>
- <span data-ttu-id="c5750-109">Jalankan perintah PowerShell [Get-CsTeamsMessagingPolicy-identitas global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) dan verifikasi bahwa **Allowgiphy** diatur ke **True**.</span><span class="sxs-lookup"><span data-stu-id="c5750-109">Run the PowerShell command [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) and verify that **AllowGiphy** is set to **TRUE**.</span></span>
- <span data-ttu-id="c5750-110">Jika **Allowgiphy** diatur ke **false** , jalankan perintah PowerShell berikut ini [set-CsTeamsMessagingPolicy-identitas Global-allowgiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="c5750-110">If **AllowGiphy** is set to **FALSE** , run the following PowerShell command [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span></span>

<span data-ttu-id="c5750-111">[Pengalaman terhubung opsional](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) perlu diaktifkan untuk memperbolehkan akses ke URL giphy.</span><span class="sxs-lookup"><span data-stu-id="c5750-111">[Optional Connected Experiences](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) need to be enabled to allow access to the Giphy URL.</span></span>

> [!NOTE]
> <span data-ttu-id="c5750-112">Jika Anda memiliki beberapa tim pesan yang dikonfigurasi untuk penyewa Anda, Anda bisa menentukan identitas kebijakan yang ditetapkan untuk pengguna yang terkena dampak dengan perintah PowerShell [Get-CsOnlineUser-identitas](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Pilih TeamsMessagingPolicy.</span><span class="sxs-lookup"><span data-stu-id="c5750-112">If you have multiple Teams Messaging policies configured for your tenant, you can determine the identity of the policy assigned to the impacted user with the PowerShell command [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Select TeamsMessagingPolicy.</span></span>
