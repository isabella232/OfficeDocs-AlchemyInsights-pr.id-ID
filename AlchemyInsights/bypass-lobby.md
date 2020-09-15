---
title: Bypass Lobby
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684953"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Mengontrol pengaturan lobi dan tingkat partisipasi di teams

Jika Anda ingin memperbolehkan semua orang, termasuk pengguna dial-in, eksternal, dan anonim, untuk **melewati lobi**, gunakan PowerShell untuk menyelesaikan tugas ini. Berikut ini adalah contoh modifikasi kebijakan Rapat global untuk organisasi Anda.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Cmdlet ini saat ini memerlukan penggunaan modul PowerShell untuk bisnis Skype. Untuk menyiapkan penggunaan cmdlet ini, lihat [mengelola kebijakan melalui PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Setelah Anda menyiapkan kebijakan, Anda perlu menerapkannya ke pengguna; atau, jika Anda mengubah kebijakan global, kebijakan tersebut akan diterapkan secara otomatis kepada pengguna. Untuk perubahan kebijakan apa pun, Anda harus menunggu setidaknya **4 jam hingga 24 jam** agar kebijakan diberlakukan. 

Pastikan untuk meninjau dokumentasi di bawah ini sebelum membuat perubahan ini untuk memahami dengan tepat apa yang memungkinkan ini.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Memahami kontrol Kebijakan lobi Rapat teams

Pengaturan ini mengontrol peserta rapat yang menunggu di lobi sebelum mereka masuk ke rapat dan tingkat partisipasi yang diperbolehkan dalam Rapat. Anda bisa menggunakan PowerShell untuk memperbarui pengaturan kebijakan Rapat yang belum diterapkan (berlabel "segera hadir") di pusat admin teams. Lihat di bawah ini untuk contoh Cmdlet PowerShell yang memperbolehkan semua pengguna untuk melewati lobi.

- [Secara otomatis mengakui orang](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) adalah kebijakan per-agenda yang mengontrol apakah orang bergabung dalam Rapat secara langsung atau menunggu di lobi hingga mereka diterima oleh pengguna yang diautentikasi.

- [Izinkan orang anonim memulai Rapat](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) adalah kebijakan per-agenda yang mengontrol apakah orang anonim, termasuk pengguna B2B dan gabungan, bisa bergabung dalam Rapat pengguna tanpa pengguna yang diautentikasi dari organisasi yang hadir.

- [Izinkan pengguna dial-in untuk melewati lobi](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**segera hadir**) adalah kebijakan per-agenda yang mengontrol apakah orang yang menelepon melalui telepon bergabung dalam Rapat secara langsung atau menunggu di lobi terlepas dari pengaturan **orang yang secara otomatis mengakui** .

- [Izinkan penyelenggara untuk mengesampingkan pengaturan lobi](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**segera hadir**) adalah kebijakan per-agenda yang mengontrol apakah penyelenggara Rapat bisa mengesampingkan pengaturan lobi yang diatur admin di **secara otomatis mengakui orang** dan **memperbolehkan pengguna dial-in untuk melewati lobi** saat mereka menjadwalkan Rapat baru.

**Catatan:** Baca [mengelola kebijakan Rapat di teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) untuk gambaran umum lengkap tentang kebijakan Rapat Microsoft teams.
