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
ms.openlocfilehash: dac6690b66181455a1c9c0f40a642b71f2af3516d91ea0853d06564b017b03a2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059599"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Mengontrol pengaturan dan tingkat partisipasi lobi Teams

Jika Anda ingin memperbolehkan semua orang, termasuk pengguna Dial-in, eksternal, dan anonim, untuk melewati lobi **,** gunakan PowerShell untuk menyelesaikan tugas ini. Berikut ini adalah contoh memodifikasi kebijakan rapat global untuk organisasi Anda.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Cmdlet ini saat ini memerlukan penggunaan Skype for Business PowerShell. Untuk bersiap menggunakan cmdlet ini, lihat [Mengelola kebijakan melalui PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Begitu Anda sudah menyiapkan kebijakan, Anda perlu menerapkannya ke pengguna; atau, jika Anda mengubah kebijakan Global, kebijakan ini akan otomatis berlaku bagi pengguna. Untuk setiap perubahan kebijakan, Anda harus menunggu **setidaknya 4 jam hingga 24** jam agar kebijakan berlaku. 

Pastikan untuk meninjau dokumentasi di bawah ini sebelum membuat perubahan ini untuk memahami apa yang mengizinkannya dengan tepat.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Memahami Teams kebijakan lobi rapat

Pengaturan ini mengontrol peserta rapat mana yang menunggu di lobi sebelum mereka masuk ke rapat dan tingkat partisipasi mereka diperbolehkan dalam rapat. Anda dapat menggunakan PowerShell untuk memperbarui pengaturan kebijakan rapat yang belum diterapkan (berlabel "segera hadir") di Teams admin baru. Lihat di bawah ini untuk contoh cmdlet PowerShell yang memungkinkan semua pengguna melewati lobi.

- [Secara otomatis memasukkan](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) orang adalah kebijakan per penyelenggara yang mengontrol apakah orang yang bergabung dalam rapat secara langsung atau menunggu di lobi hingga mereka dibawa oleh pengguna yang diautentikasi.

- [Perbolehkan](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) orang anonim memulai rapat adalah kebijakan per penyelenggara yang mengontrol apakah orang-orang anonim, termasuk B2B dan pengguna gabungan, bisa bergabung dalam rapat pengguna tanpa pengguna terautentikasi dari organisasi secara kehadiran.

- Memperbolehkan pengguna [dial-in](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) melewati lobi **(** segera hadir ) adalah kebijakan per penyelenggara yang mengontrol apakah orang yang menghubungi dengan telepon akan langsung bergabung atau menunggu di lobi terlepas dari pengaturan Memasukkan orang **secara** otomatis.

- Izinkan [penyelenggara](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) untuk menimpa pengaturan lobi **(** segera hadir ) adalah kebijakan per penyelenggara yang mengontrol apakah  penyelenggara rapat dapat menimpa pengaturan lobi yang diatur admin dalam Memasukkan orang dan Memperbolehkan pengguna **dial-in** secara otomatis melewati lobi ketika menjadwalkan rapat baru.

**Catatan:** Baca [Mengelola kebijakan rapat di Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) untuk gambaran umum lengkap Microsoft Teams rapat.
