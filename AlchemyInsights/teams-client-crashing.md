---
title: Klien Teams mengalami crash?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ac1cc05adfa33626ff34d30dca6c77f1bb96477a
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354055"
---
# <a name="teams-client-crashing"></a>Klien Teams mengalami crash?

Jika klien Teams Anda mengalami crash, cobalah langkah berikut:

- Jika Anda menggunakan aplikasi desktop Teams, [pastikan aplikasi sudah diperbarui sepenuhnya](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Pastikan semua [Microsoft 365 URL dan kisaran alamat](https://docs.microsoft.com/microsoftteams/connectivity-issues) dapat diakses.

- Masuk dengan akun admin penyewa Anda dan periksa [dasbor Kesehatan Layanan](https://docs.microsoft.com/office365/enterprise/view-service-health) Anda untuk memverifikasi bahwa tidak ada pemutusan atau degradasi layanan yang ada.

- Uninstall dan menginstal ulang teams aplikasi (link)
    - Browse ke folder%appdata%\Microsoft\teams\ di komputer Anda dan menghapus semua file dalam direktori tersebut.
    - [Unduh dan instal aplikasi teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), dan jika memungkinkan, instal teams sebagai administrator (klik kanan Penginstal teams, lalu pilih "Jalankan sebagai administrator" jika tersedia).

Jika klien tim Anda masih mogok, Dapatkah Anda mereproduksi masalah? Jika demikian:

1. Gunakan langkah Recorder untuk menangkap langkah Anda.
    - Tutup semua aplikasi yang tidak perlu atau rahasia.
    - Peluncuran langkah Recorder dan mereproduksi masalah saat masuk dengan akun pengguna yang dipakai.
    - [Mengumpulkan log tim yang menangkap langkah repro direkam](https://docs.microsoft.com/microsoftteams/log-files). **Catatan**: Pastikan Anda menangkap alamat masuk dari pengguna yang terkena dampak.
    - Mengumpulkan dump dan/atau kesalahan ember info (Windows). Luncurkan Windows PowerShell di mesin tempat terjadinya crash dan jalankan perintah berikut:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Lampirkan file ke kasus dukungan Anda.
