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
ms.openlocfilehash: de665ca6defcd0d00d227435473e5a4ccf61bc82
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376693"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="87e2b-102">Pengaturan lobi kontrol dan tingkat partisipasi</span><span class="sxs-lookup"><span data-stu-id="87e2b-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="87e2b-103">Pengaturan ini mengontrol yang peserta pertemuan menunggu di lobi sebelum mereka diterima Rapat dan tingkat partisipasi mereka diperbolehkan dalam pertemuan.</span><span class="sxs-lookup"><span data-stu-id="87e2b-103">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="87e2b-104">Anda dapat menggunakan PowerShell untuk memperbarui pengaturan kebijakan pertemuan yang belum diterapkan (berlabel "segera hadir") di pusat admin teams.</span><span class="sxs-lookup"><span data-stu-id="87e2b-104">You can use Powershell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span>  <span data-ttu-id="87e2b-105">Lihat di bawah ini untuk contoh PowerShell cmdlet yang memungkinkan semua pengguna untuk melewati lobi.</span><span class="sxs-lookup"><span data-stu-id="87e2b-105">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>  

- <span data-ttu-id="87e2b-106">[Secara otomatis mengakui orang](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) adalah kebijakan per penyelenggara yang mengontrol apakah orang bergabung dengan Rapat secara langsung atau menunggu di lobi sampai mereka diterima oleh pengguna yang diotentikasi.</span><span class="sxs-lookup"><span data-stu-id="87e2b-106">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="87e2b-107">[Izinkan orang anonim untuk memulai pertemuan](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) adalah kebijakan per penyelenggara yang mengontrol apakah orang anonim, termasuk B2B dan pengguna Federasi, dapat bergabung dengan Rapat pengguna tanpa pengguna yang diotentikasi dari organisasi yang hadir.</span><span class="sxs-lookup"><span data-stu-id="87e2b-107">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="87e2b-108">[Izinkan pengguna panggilan masuk untuk melewati lobi](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (segera**hadir**) adalah kebijakan per penyelenggara yang mengontrol apakah orang yang melakukan panggilan telepon bergabung dengan Rapat secara langsung atau menunggu di lobi tanpa menghiraukan pengaturan **orang secara otomatis** .</span><span class="sxs-lookup"><span data-stu-id="87e2b-108">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="87e2b-109">[Memungkinkan penyelenggara untuk menimpa setelan lobi](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (segera**hadir**) adalah kebijakan per penyelenggara yang mengontrol apakah penyelenggara pertemuan dapat menimpa setelan lobi yang diatur admin **secara otomatis mengakui orang** dan **mengizinkan panggilan masuk pengguna untuk melewati lobi** saat mereka menjadwalkan pertemuan baru.</span><span class="sxs-lookup"><span data-stu-id="87e2b-109">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="87e2b-110">**Catatan:** Baca [mengelola kebijakan Rapat di teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) untuk Ikhtisar lengkap tentang kebijakan Rapat Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="87e2b-110">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span> 


<span data-ttu-id="87e2b-111">**Contoh PowerShell**</span><span class="sxs-lookup"><span data-stu-id="87e2b-111">**PowerShell example**</span></span>

<span data-ttu-id="87e2b-112">Jika Anda ingin mengizinkan semua orang, termasuk pengguna eksternal atau anonim, untuk melewati lobi, Anda juga dapat menggunakan PowerShell untuk menyelesaikan tugas ini.</span><span class="sxs-lookup"><span data-stu-id="87e2b-112">If you'd like to allow everyone, including external or anonymous users, to bypass the lobby, you can also use PowerShell to accomplish this task.</span></span>  <span data-ttu-id="87e2b-113">Berikut adalah contoh memodifikasi Kebijakan pertemuan global untuk organisasi Anda.</span><span class="sxs-lookup"><span data-stu-id="87e2b-113">Here's an example of modifying the global meeting policy for your organization.</span></span>   

<span data-ttu-id="87e2b-114">(Pastikan untuk meninjau dokumentasi di atas sebelum membuat perubahan ini untuk memahami dengan tepat apa yang memungkinkan.)</span><span class="sxs-lookup"><span data-stu-id="87e2b-114">(Be sure to review the documentation above before making these changes to understand exactly what this allows.)</span></span>

<span data-ttu-id="87e2b-115">Set-CsTeamsMeetingPolicy-identitas global-AutoAdmittedUsers "semua orang"-AllowPSTNUsersToBypassLobby $True</span><span class="sxs-lookup"><span data-stu-id="87e2b-115">Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True</span></span>

<span data-ttu-id="87e2b-116">Untuk informasi selengkapnya, lihat [set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="87e2b-116">For more information, see [Set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span></span>
