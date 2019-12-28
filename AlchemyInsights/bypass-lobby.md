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
ms.openlocfilehash: 311af365a94b788182bb6870bca3f67b2ad802d0
ms.sourcegitcommit: 932981641dd8e973e28dfe346bbdf9c923111b13
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/27/2019
ms.locfileid: "40889085"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="bf6d4-102">Pengaturan lobi kontrol dan tingkat partisipasi di teams</span><span class="sxs-lookup"><span data-stu-id="bf6d4-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="bf6d4-103">Jika Anda ingin mengizinkan semua orang, termasuk pengguna panggilan masuk, eksternal, dan anonim, untuk **melewati lobi**, gunakan PowerShell untuk menyelesaikan tugas ini.</span><span class="sxs-lookup"><span data-stu-id="bf6d4-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="bf6d4-104">Berikut adalah contoh memodifikasi Kebijakan pertemuan global untuk organisasi Anda.</span><span class="sxs-lookup"><span data-stu-id="bf6d4-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="bf6d4-105">Cmdlet ini saat ini memerlukan penggunaan Skype untuk bisnis PowerShell modul.</span><span class="sxs-lookup"><span data-stu-id="bf6d4-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="bf6d4-106">Untuk mendapatkan pengaturan untuk menggunakan cmdlet ini, periksa [mengelola kebijakan melalui PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="bf6d4-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="bf6d4-107">Setelah Anda menyiapkan kebijakan, Anda harus menerapkannya pada pengguna; atau, jika Anda memodifikasi Kebijakan global, maka secara otomatis akan berlaku untuk pengguna.</span><span class="sxs-lookup"><span data-stu-id="bf6d4-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="bf6d4-108">Untuk setiap perubahan kebijakan, Anda harus menunggu setidaknya **4 jam hingga 24 jam** agar kebijakan diterapkan.</span><span class="sxs-lookup"><span data-stu-id="bf6d4-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="bf6d4-109">Pastikan untuk meninjau dokumentasi di bawah ini sebelum membuat perubahan ini untuk memahami dengan tepat apa yang memungkinkan ini.</span><span class="sxs-lookup"><span data-stu-id="bf6d4-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="bf6d4-110">Memahami kontrol Kebijakan lobi Rapat tim</span><span class="sxs-lookup"><span data-stu-id="bf6d4-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="bf6d4-111">Pengaturan ini mengontrol yang peserta pertemuan menunggu di lobi sebelum mereka diterima Rapat dan tingkat partisipasi mereka diperbolehkan dalam pertemuan.</span><span class="sxs-lookup"><span data-stu-id="bf6d4-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="bf6d4-112">Anda dapat menggunakan PowerShell untuk memperbarui pengaturan kebijakan pertemuan yang belum diterapkan (berlabel "segera hadir") di pusat admin teams.</span><span class="sxs-lookup"><span data-stu-id="bf6d4-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="bf6d4-113">Lihat di bawah ini untuk contoh PowerShell cmdlet yang memungkinkan semua pengguna untuk melewati lobi.</span><span class="sxs-lookup"><span data-stu-id="bf6d4-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="bf6d4-114">[Secara otomatis mengakui orang](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) adalah kebijakan per penyelenggara yang mengontrol apakah orang bergabung dengan Rapat secara langsung atau menunggu di lobi sampai mereka diterima oleh pengguna yang diotentikasi.</span><span class="sxs-lookup"><span data-stu-id="bf6d4-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="bf6d4-115">[Izinkan orang anonim untuk memulai pertemuan](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) adalah kebijakan per penyelenggara yang mengontrol apakah orang anonim, termasuk B2B dan pengguna Federasi, dapat bergabung dengan Rapat pengguna tanpa pengguna yang diotentikasi dari organisasi yang hadir.</span><span class="sxs-lookup"><span data-stu-id="bf6d4-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="bf6d4-116">[Izinkan pengguna panggilan masuk untuk melewati lobi](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (segera**hadir**) adalah kebijakan per penyelenggara yang mengontrol apakah orang yang melakukan panggilan telepon bergabung dengan Rapat secara langsung atau menunggu di lobi tanpa menghiraukan pengaturan **orang secara otomatis** .</span><span class="sxs-lookup"><span data-stu-id="bf6d4-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="bf6d4-117">[Memungkinkan penyelenggara untuk menimpa setelan lobi](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (segera**hadir**) adalah kebijakan per penyelenggara yang mengontrol apakah penyelenggara pertemuan dapat menimpa setelan lobi yang diatur admin secara **otomatis mengakui orang** dan **mengizinkan pengguna panggilan masuk untuk melewati lobi** saat mereka menjadwalkan pertemuan baru.</span><span class="sxs-lookup"><span data-stu-id="bf6d4-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="bf6d4-118">**Catatan:** Baca [mengelola kebijakan Rapat di teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) untuk Ikhtisar lengkap tentang kebijakan Rapat Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="bf6d4-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
