---
title: Klien Teams mengalami crash?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826274"
---
# <a name="teams-client-crashing"></a>Klien Teams mengalami crash?

Jika klien Teams Anda mengalami crash, cobalah langkah berikut:

- Jika Anda menggunakan aplikasi desktop Teams, [pastikan aplikasi sudah diperbarui sepenuhnya](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Pastikan semua rentang [alamat dan URL Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) mudah diakses.

- Masuk dengan akun admin penyewa Anda dan periksa Dasbor [Kesehatan Layanan Anda untuk](https://docs.microsoft.com/office365/enterprise/view-service-health) memastikan bahwa tidak ada gangguan atau degradasi layanan.

- Menghapus instalan dan menginstal ulang Aplikasi Teams (tautan)
    - Telusuri ke folder %appdata%\Microsoft\teams\ di komputer Anda dan hapus semua file dalam direktori tersebut.
    - [Unduh dan instal Aplikasi Teams,](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)dan jika memungkinkan, instal Teams sebagai administrator (klik kanan penginstal Teams, lalu pilih "Jalankan sebagai administrator" jika tersedia).

Jika klien Teams masih mengalami crash, dapatkah Anda mereproduksi masalah? Jika demikian:

1. Gunakan Perekam Langkah untuk merekam langkah Anda.
    - Tutup SEMUA aplikasi yang tidak diperlukan atau rahasia.
    - Luncurkan Perekam Langkah dan mereproduksi masalah saat masuk dengan akun pengguna yang terpengaruh.
    - [Kumpulkan log tim yang merekam langkah-langkah profesional yang direkam.](https://docs.microsoft.com/microsoftteams/log-files) **Catatan**: Pastikan Anda mencatat alamat masuk pengguna yang terkena dampak.
    - Kumpulkan buang dan/atau Info wadah kesalahan (Windows). Luncurkan Windows Powershell di komputer tempat crash terjadi dan jalankan perintah berikut:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Lampirkan file ke kasus dukungan Anda.
