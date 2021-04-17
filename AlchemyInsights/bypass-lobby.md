---
title: Melewati lobi
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
- "2673"
- "9000740"
ms.openlocfilehash: bcb40c6f15e957c0a59911322c3b28f03cd562c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820037"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="0fb5a-102">Mengontrol pengaturan dan tingkat partisipasi lobi di Teams</span><span class="sxs-lookup"><span data-stu-id="0fb5a-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="0fb5a-103">Jika Anda ingin memperbolehkan semua orang, termasuk pengguna Dial-in, eksternal, dan anonim, untuk melewati lobi **,** gunakan PowerShell untuk menyelesaikan tugas ini.</span><span class="sxs-lookup"><span data-stu-id="0fb5a-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="0fb5a-104">Berikut ini adalah contoh memodifikasi kebijakan rapat global untuk organisasi Anda.</span><span class="sxs-lookup"><span data-stu-id="0fb5a-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="0fb5a-105">Cmdlet ini saat ini memerlukan penggunaan modul Skype for Business PowerShell.</span><span class="sxs-lookup"><span data-stu-id="0fb5a-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="0fb5a-106">Untuk bersiap menggunakan cmdlet ini, lihat [Mengelola kebijakan melalui PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="0fb5a-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="0fb5a-107">Begitu Anda sudah menyiapkan kebijakan, Anda perlu menerapkannya ke pengguna; atau, jika Anda mengubah kebijakan Global, kebijakan ini akan otomatis berlaku bagi pengguna.</span><span class="sxs-lookup"><span data-stu-id="0fb5a-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="0fb5a-108">Untuk setiap perubahan kebijakan, Anda harus menunggu **setidaknya 4 jam hingga 24** jam agar kebijakan berlaku.</span><span class="sxs-lookup"><span data-stu-id="0fb5a-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="0fb5a-109">Pastikan untuk meninjau dokumentasi di bawah ini sebelum membuat perubahan ini untuk memahami apa yang mengizinkannya dengan tepat.</span><span class="sxs-lookup"><span data-stu-id="0fb5a-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="0fb5a-110">Memahami kontrol kebijakan lobi rapat Teams</span><span class="sxs-lookup"><span data-stu-id="0fb5a-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="0fb5a-111">Pengaturan ini mengontrol peserta rapat mana yang menunggu di lobi sebelum mereka masuk ke rapat dan tingkat partisipasi mereka diperbolehkan dalam rapat.</span><span class="sxs-lookup"><span data-stu-id="0fb5a-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="0fb5a-112">Anda dapat menggunakan PowerShell untuk memperbarui pengaturan kebijakan rapat yang belum diterapkan (berlabel "segera hadir") di pusat admin Teams.</span><span class="sxs-lookup"><span data-stu-id="0fb5a-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="0fb5a-113">Lihat di bawah ini untuk contoh cmdlet PowerShell yang memungkinkan semua pengguna melewati lobi.</span><span class="sxs-lookup"><span data-stu-id="0fb5a-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="0fb5a-114">[Secara otomatis memasukkan](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) orang adalah kebijakan per penyelenggara yang mengontrol apakah orang yang bergabung dalam rapat secara langsung atau menunggu di lobi hingga mereka dibawa oleh pengguna yang diautentikasi.</span><span class="sxs-lookup"><span data-stu-id="0fb5a-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="0fb5a-115">[Perbolehkan](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) orang anonim memulai rapat adalah kebijakan per penyelenggara yang mengontrol apakah orang-orang anonim, termasuk B2B dan pengguna gabungan, bisa bergabung dalam rapat pengguna tanpa pengguna terautentikasi dari organisasi secara kehadiran.</span><span class="sxs-lookup"><span data-stu-id="0fb5a-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="0fb5a-116">Memperbolehkan pengguna [dial-in](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) melewati lobi **(** segera hadir ) adalah kebijakan per penyelenggara yang mengontrol apakah orang yang menghubungi dengan telepon akan langsung bergabung atau menunggu di lobi terlepas dari pengaturan Memasukkan orang **secara** otomatis.</span><span class="sxs-lookup"><span data-stu-id="0fb5a-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="0fb5a-117">Izinkan [penyelenggara](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) untuk menimpa pengaturan lobi **(** segera hadir ) adalah kebijakan per penyelenggara yang mengontrol apakah  penyelenggara rapat dapat menimpa pengaturan lobi yang diatur admin dalam Memasukkan orang dan Memperbolehkan pengguna **dial-in** secara otomatis melewati lobi ketika menjadwalkan rapat baru.</span><span class="sxs-lookup"><span data-stu-id="0fb5a-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="0fb5a-118">**Catatan:** Baca [Mengelola kebijakan rapat di Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) untuk gambaran umum lengkap tentang kebijakan rapat Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="0fb5a-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
