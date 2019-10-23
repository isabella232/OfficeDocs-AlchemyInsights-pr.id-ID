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
ms.openlocfilehash: 729fc5d4213acbbdf74a9d07adacb42b34170717
ms.sourcegitcommit: ffbeb72c9199ab4ebcb0f1ad443ed3e2f4950efc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/23/2019
ms.locfileid: "37637780"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>Pengaturan lobi kontrol dan tingkat partisipasi

Jika Anda ingin mengizinkan semua orang, termasuk pengguna panggilan masuk, eksternal, dan anonim untuk melewati lobi, Anda dapat menggunakan PowerShell untuk melakukannya. Berikut adalah contoh memodifikasi Kebijakan pertemuan global untuk organisasi Anda:

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Cmdlet ini saat ini memerlukan penggunaan Skype untuk bisnis PowerShell modul. Untuk mendapatkan penyiapan untuk menggunakan cmdlet ini, lihat Mengelola Kebijakan melalui PowerShell.

Anda dapat menyiapkan kebijakan baru, yang kemudian harus diterapkan ke pengguna. Jika Anda mengubah kebijakan global itu secara otomatis akan berlaku untuk pengguna. Untuk setiap perubahan kebijakan, Anda harus menunggu setidaknya 4 jam dan hingga 24 jam agar kebijakan diterapkan.

Pastikan untuk meninjau dokumentasi di bawah ini sebelum membuat perubahan ini untuk memahami dengan tepat apa yang memungkinkan ini.

## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Memahami kontrol Kebijakan lobi Rapat tim

- [Secara otomatis mengakui orang](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) adalah kebijakan per penyelenggara yang mengontrol apakah orang bergabung dengan Rapat secara langsung atau menunggu di lobi sampai mereka diterima oleh pengguna yang diotentikasi.

- [Izinkan orang anonim untuk memulai pertemuan](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) adalah kebijakan per penyelenggara yang mengontrol apakah orang anonim, termasuk B2B dan pengguna Federasi, dapat bergabung dengan Rapat pengguna tanpa pengguna yang diotentikasi dari organisasi yang hadir.

- [Izinkan pengguna panggilan masuk untuk melewati lobi](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (segera**hadir**) adalah kebijakan per penyelenggara yang mengontrol apakah orang yang melakukan panggilan telepon bergabung dengan Rapat secara langsung atau menunggu di lobi tanpa menghiraukan pengaturan **orang secara otomatis** .

- [Memungkinkan penyelenggara untuk menimpa setelan lobi](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (segera**hadir**) adalah kebijakan per penyelenggara yang mengontrol apakah penyelenggara pertemuan dapat menimpa setelan lobi yang diatur admin **secara otomatis mengakui orang** dan **mengizinkan panggilan masuk pengguna untuk melewati lobi** saat mereka menjadwalkan pertemuan baru.

**Catatan:** Baca [mengelola kebijakan Rapat di teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) untuk Ikhtisar lengkap tentang kebijakan Rapat Microsoft teams.
