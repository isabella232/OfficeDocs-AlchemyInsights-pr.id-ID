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
# <a name="control-lobby-settings-and-level-of-participation"></a>Pengaturan lobi kontrol dan tingkat partisipasi

Pengaturan ini mengontrol yang peserta pertemuan menunggu di lobi sebelum mereka diterima Rapat dan tingkat partisipasi mereka diperbolehkan dalam pertemuan. Anda dapat menggunakan PowerShell untuk memperbarui pengaturan kebijakan pertemuan yang belum diterapkan (berlabel "segera hadir") di pusat admin teams.  Lihat di bawah ini untuk contoh PowerShell cmdlet yang memungkinkan semua pengguna untuk melewati lobi.  

- [Secara otomatis mengakui orang](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) adalah kebijakan per penyelenggara yang mengontrol apakah orang bergabung dengan Rapat secara langsung atau menunggu di lobi sampai mereka diterima oleh pengguna yang diotentikasi.

- [Izinkan orang anonim untuk memulai pertemuan](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) adalah kebijakan per penyelenggara yang mengontrol apakah orang anonim, termasuk B2B dan pengguna Federasi, dapat bergabung dengan Rapat pengguna tanpa pengguna yang diotentikasi dari organisasi yang hadir.

- [Izinkan pengguna panggilan masuk untuk melewati lobi](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (segera**hadir**) adalah kebijakan per penyelenggara yang mengontrol apakah orang yang melakukan panggilan telepon bergabung dengan Rapat secara langsung atau menunggu di lobi tanpa menghiraukan pengaturan **orang secara otomatis** .

- [Memungkinkan penyelenggara untuk menimpa setelan lobi](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (segera**hadir**) adalah kebijakan per penyelenggara yang mengontrol apakah penyelenggara pertemuan dapat menimpa setelan lobi yang diatur admin **secara otomatis mengakui orang** dan **mengizinkan panggilan masuk pengguna untuk melewati lobi** saat mereka menjadwalkan pertemuan baru.

**Catatan:** Baca [mengelola kebijakan Rapat di teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) untuk Ikhtisar lengkap tentang kebijakan Rapat Microsoft teams. 


**Contoh PowerShell**

Jika Anda ingin mengizinkan semua orang, termasuk pengguna eksternal atau anonim, untuk melewati lobi, Anda juga dapat menggunakan PowerShell untuk menyelesaikan tugas ini.  Berikut adalah contoh memodifikasi Kebijakan pertemuan global untuk organisasi Anda.   

(Pastikan untuk meninjau dokumentasi di atas sebelum membuat perubahan ini untuk memahami dengan tepat apa yang memungkinkan.)

Set-CsTeamsMeetingPolicy-identitas global-AutoAdmittedUsers "semua orang"-AllowPSTNUsersToBypassLobby $True

Untuk informasi selengkapnya, lihat [set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).
