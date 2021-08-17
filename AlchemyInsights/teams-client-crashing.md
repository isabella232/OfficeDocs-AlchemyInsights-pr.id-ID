---
title: Teams mengalami crash
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
ms.openlocfilehash: a292e160abcfc26ffebc454d32ee489a319a23f4bb81e70fe5dbe72bfd0b8b81
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890341"
---
# <a name="teams-client-crashing"></a>Teams mengalami crash

Jika klien Teams Anda mengalami crash, cobalah langkah berikut:

- Jika Anda menggunakan aplikasi desktop Teams, [pastikan aplikasi sudah diperbarui sepenuhnya](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Pastikan semua [rentang Microsoft 365 URL dan alamat mudah](https://docs.microsoft.com/microsoftteams/connectivity-issues) diakses.

- Masuk dengan akun admin penyewa Anda dan periksa Dasbor [Kesehatan Layanan Anda untuk](https://docs.microsoft.com/office365/enterprise/view-service-health) memastikan bahwa tidak ada gangguan atau degradasi layanan.

- Menghapus instalan dan menginstal Teams Instalan
    - Telusuri ke folder %appdata%\Microsoft\Teams\ di komputer Anda dan hapus semua file dalam direktori tersebut.
    - [Unduh dan instal Aplikasi Teams,](https://www.microsoft.com/microsoft-teams/download-app)dan jika memungkinkan, instal Teams sebagai administrator (klik kanan penginstal Teams, lalu pilih Jalankan **sebagai administrator** jika tersedia).

Jika klien Teams mengalami crash, cobalah untuk mereproduksi masalah. Jika Anda bisa:

1. Gunakan Perekam Langkah untuk merekam langkah Anda.
    - Tutup SEMUA aplikasi yang tidak diperlukan atau rahasia.
    - Luncurkan Perekam Langkah dan mereproduksi masalah saat masuk dengan akun pengguna yang terpengaruh.
    - [Kumpulkan log tim yang merekam langkah-langkah profesional yang direkam.](https://docs.microsoft.com/microsoftteams/log-files) **Catatan**: Pastikan Anda mencatat alamat masuk pengguna yang terkena dampak.
    - Kumpulkan buang dan/atau Info wadah kesalahan (Windows). Luncurkan Windows Powershell di komputer tempat crash terjadi dan jalankan perintah berikut (setelah setiap perintah, tekan Enter):

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. Setelah file teks dibuat dan muncul di layar Anda, simpan file dan lampirkan ke permintaan layanan. 
