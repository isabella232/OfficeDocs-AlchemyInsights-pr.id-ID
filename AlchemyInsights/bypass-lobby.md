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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Pengaturan lobi kontrol dan tingkat partisipasi di teams

Jika Anda ingin mengizinkan semua orang, termasuk pengguna panggilan masuk, eksternal, dan anonim, untuk **melewati lobi**, gunakan PowerShell untuk menyelesaikan tugas ini. Berikut adalah contoh memodifikasi Kebijakan pertemuan global untuk organisasi Anda.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Cmdlet ini saat ini memerlukan penggunaan Skype untuk bisnis PowerShell modul. Untuk mendapatkan pengaturan untuk menggunakan cmdlet ini, periksa [mengelola kebijakan melalui PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Setelah Anda menyiapkan kebijakan, Anda harus menerapkannya pada pengguna; atau, jika Anda memodifikasi Kebijakan global, maka secara otomatis akan berlaku untuk pengguna. Untuk setiap perubahan kebijakan, Anda harus menunggu setidaknya **4 jam hingga 24 jam** agar kebijakan diterapkan. 

Pastikan untuk meninjau dokumentasi di bawah ini sebelum membuat perubahan ini untuk memahami dengan tepat apa yang memungkinkan ini.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Memahami kontrol Kebijakan lobi Rapat tim

Pengaturan ini mengontrol yang peserta pertemuan menunggu di lobi sebelum mereka diterima Rapat dan tingkat partisipasi mereka diperbolehkan dalam pertemuan. Anda dapat menggunakan PowerShell untuk memperbarui pengaturan kebijakan pertemuan yang belum diterapkan (berlabel "segera hadir") di pusat admin teams. Lihat di bawah ini untuk contoh PowerShell cmdlet yang memungkinkan semua pengguna untuk melewati lobi.

- [Secara otomatis mengakui orang](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) adalah kebijakan per penyelenggara yang mengontrol apakah orang bergabung dengan Rapat secara langsung atau menunggu di lobi sampai mereka diterima oleh pengguna yang diotentikasi.

- [Izinkan orang anonim untuk memulai pertemuan](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) adalah kebijakan per penyelenggara yang mengontrol apakah orang anonim, termasuk B2B dan pengguna Federasi, dapat bergabung dengan Rapat pengguna tanpa pengguna yang diotentikasi dari organisasi yang hadir.

- [Izinkan pengguna panggilan masuk untuk melewati lobi](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (segera**hadir**) adalah kebijakan per penyelenggara yang mengontrol apakah orang yang melakukan panggilan telepon bergabung dengan Rapat secara langsung atau menunggu di lobi tanpa menghiraukan pengaturan **orang secara otomatis** .

- [Memungkinkan penyelenggara untuk menimpa setelan lobi](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (segera**hadir**) adalah kebijakan per penyelenggara yang mengontrol apakah penyelenggara pertemuan dapat menimpa setelan lobi yang diatur admin secara **otomatis mengakui orang** dan **mengizinkan pengguna panggilan masuk untuk melewati lobi** saat mereka menjadwalkan pertemuan baru.

**Catatan:** Baca [mengelola kebijakan Rapat di teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) untuk Ikhtisar lengkap tentang kebijakan Rapat Microsoft teams.
