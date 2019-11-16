---
title: Bypass lobi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: bf8be9ffe2bfa45ed2cf149c1c4fa118b40e816d
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768443"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="9ce63-102">Pengaturan lobi kontrol dan tingkat partisipasi</span><span class="sxs-lookup"><span data-stu-id="9ce63-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="9ce63-103">Jika Anda ingin mengizinkan semua orang, termasuk pengguna panggilan masuk, eksternal, dan anonim untuk melewati lobi di Microsoft teams, Anda dapat menggunakan PowerShell untuk melakukannya.</span><span class="sxs-lookup"><span data-stu-id="9ce63-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users to bypass the lobby in Microsoft Teams, you can use PowerShell to do it.</span></span> <span data-ttu-id="9ce63-104">Berikut adalah contoh memodifikasi Kebijakan pertemuan global untuk organisasi Anda:</span><span class="sxs-lookup"><span data-stu-id="9ce63-104">Here's an example of modifying the global meeting policy for your organization:</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="9ce63-105">Cmdlet ini saat ini memerlukan penggunaan Skype untuk bisnis PowerShell modul.</span><span class="sxs-lookup"><span data-stu-id="9ce63-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="9ce63-106">Untuk mendapatkan pengaturan untuk menggunakan cmdlet ini, periksa [mengelola kebijakan melalui PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="9ce63-106">To get setup to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="9ce63-107">Anda dapat menyiapkan kebijakan baru, yang kemudian harus diterapkan ke pengguna.</span><span class="sxs-lookup"><span data-stu-id="9ce63-107">You can set up a new policy, which you'll then need to apply it to users.</span></span> <span data-ttu-id="9ce63-108">Jika Anda mengubah kebijakan global itu secara otomatis akan berlaku untuk pengguna.</span><span class="sxs-lookup"><span data-stu-id="9ce63-108">If you modify the Global policy it'll automatically apply to users.</span></span> <span data-ttu-id="9ce63-109">Untuk setiap perubahan kebijakan, Anda harus menunggu setidaknya 4 jam dan hingga 24 jam agar kebijakan diterapkan.</span><span class="sxs-lookup"><span data-stu-id="9ce63-109">For any policy change you need to wait at least 4 hours and up to 24 hours for the policies to take effect.</span></span>

<span data-ttu-id="9ce63-110">Pastikan untuk meninjau dokumentasi di bawah ini sebelum membuat perubahan ini untuk memahami dengan tepat apa yang memungkinkan ini.</span><span class="sxs-lookup"><span data-stu-id="9ce63-110">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>

## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="9ce63-111">Memahami kontrol Kebijakan lobi Rapat tim</span><span class="sxs-lookup"><span data-stu-id="9ce63-111">Understanding Teams meeting lobby policy controls</span></span>

- <span data-ttu-id="9ce63-112">[Secara otomatis mengakui orang](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) adalah kebijakan per penyelenggara yang mengontrol apakah orang bergabung dengan Rapat secara langsung atau menunggu di lobi sampai mereka diterima oleh pengguna yang diotentikasi.</span><span class="sxs-lookup"><span data-stu-id="9ce63-112">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="9ce63-113">[Izinkan orang anonim untuk memulai pertemuan](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) adalah kebijakan per penyelenggara yang mengontrol apakah orang anonim, termasuk B2B dan pengguna Federasi, dapat bergabung dengan Rapat pengguna tanpa pengguna yang diotentikasi dari organisasi yang hadir.</span><span class="sxs-lookup"><span data-stu-id="9ce63-113">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="9ce63-114">[Izinkan pengguna panggilan masuk untuk melewati lobi](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (segera**hadir**) adalah kebijakan per penyelenggara yang mengontrol apakah orang yang melakukan panggilan telepon bergabung dengan Rapat secara langsung atau menunggu di lobi tanpa menghiraukan pengaturan **orang secara otomatis** .</span><span class="sxs-lookup"><span data-stu-id="9ce63-114">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="9ce63-115">[Memungkinkan penyelenggara untuk menimpa setelan lobi](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (segera**hadir**) adalah kebijakan per penyelenggara yang mengontrol apakah penyelenggara pertemuan dapat menimpa setelan lobi yang diatur admin secara **otomatis mengakui orang** dan **mengizinkan pengguna panggilan masuk untuk melewati lobi** saat mereka menjadwalkan pertemuan baru.</span><span class="sxs-lookup"><span data-stu-id="9ce63-115">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="9ce63-116">**Catatan:** Baca [mengelola kebijakan Rapat di teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) untuk Ikhtisar lengkap tentang kebijakan Rapat Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="9ce63-116">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
