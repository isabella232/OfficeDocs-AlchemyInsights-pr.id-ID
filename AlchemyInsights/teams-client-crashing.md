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
ms.openlocfilehash: 7acb2f5f87a9cfbd67cd94efca696665fd80fc4a
ms.sourcegitcommit: 3cdfde87b7311c200431196031af92c640fd0d8d
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/29/2021
ms.locfileid: "53187724"
---
# <a name="teams-client-crashing"></a>Teams mengalami crash

Jika klien Teams Anda mengalami crash, cobalah langkah berikut:

- Jika Anda menggunakan aplikasi desktop Teams, [pastikan aplikasi sudah diperbarui sepenuhnya](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Pastikan semua rentang [Microsoft 365 URL dan alamat mudah](/microsoftteams/connectivity-issues) diakses.

- Masuk dengan akun admin penyewa Anda dan periksa Dasbor [Kesehatan Layanan Anda untuk](/office365/enterprise/view-service-health) memastikan bahwa tidak ada gangguan atau degradasi layanan.

- Menghapus instalasi dan menginstal ulang Teams Aplikasi
    - Telusuri ke folder %appdata%\Microsoft\Teams\ di komputer Anda dan hapus semua file dalam direktori tersebut.
    - [Unduh dan instal Aplikasi Teams](https://www.microsoft.com/microsoft-teams/download-app), dan jika memungkinkan, instal Teams sebagai administrator (klik kanan penginstal Teams, lalu pilih Jalankan sebagai **administrator** jika tersedia).

Jika klien Teams mengalami crash, cobalah untuk mereproduksi masalah. Jika Anda bisa:

1. Gunakan Perekam Langkah untuk merekam langkah Anda.
    - Tutup SEMUA aplikasi yang tidak diperlukan atau rahasia.
    - Luncurkan Perekam Langkah dan mereproduksi masalah saat masuk dengan akun pengguna yang terpengaruh.
    - [Kumpulkan log tim yang merekam langkah-langkah profesional yang direkam.](/microsoftteams/log-files) **Catatan**: Pastikan Anda mencatat alamat masuk pengguna yang terkena dampak.
    - Kumpulkan buang dan/atau Info wadah kesalahan (Windows). Luncurkan Windows Powershell di komputer tempat crash terjadi dan jalankan perintah berikut (setelah setiap perintah, tekan Enter):

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. Setelah file teks dibuat dan muncul di layar Anda, simpan file dan lampirkan ke permintaan layanan. 
