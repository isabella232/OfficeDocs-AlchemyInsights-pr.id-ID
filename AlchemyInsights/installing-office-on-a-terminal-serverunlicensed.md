---
title: Menginstal Office di terminal server-tidak berlisensi
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 53071224a7c33532d864cd70b84bf0e3cc6a992f
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/04/2019
ms.locfileid: "36735392"
---
# <a name="installing-office-on-a-terminal-server"></a>Menginstal Office di terminal server

Untuk menyebarkan Office 365 ProPlus di Windows Server menggunakan layanan desktop jarak jauh (RDS), sebelumnya bernama Layanan Terminal:
  
- Anda harus memiliki rencana Office 365 yang mencakup Office 365 ProPlus, seperti Office 365 Enterprise E3 atau Enterprise E5. Office 365 bisnis dan Office 365 rencana bisnis Premium tidak termasuk Office 365 ProPlus.

- Anda harus mengaktifkan [aktivasi komputer bersama](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

Jika Anda ingin menginstal Office 365 ProPlus di RDS dari Microsoft 365 Admin Center, ***yang menggunakan pengaturan instalasi default***, ikuti langkah-langkah berikut:
  
1. Periksa apa Office 365 rencana yang Anda miliki. [Pelajari caranya](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Jika perlu, beralih ke rencana Office 365 yang berbeda. [Pelajari caranya](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Jika Office sudah diinstal di RDS server menggunakan rencana Office 365 lainnya, bongkar. Sebagai contoh, dengan pergi ke Control Panel \> Uninstall program. Membongkar menggunakan [dukungan Microsoft dan pemulihan asisten](https://aka.ms/SARA-OfficeUninstall-Alchemy) jika Anda menjalankan ke masalah.

4. Di RDS server, masuk ke Microsoft 365 Admin Center dengan akun administrator dan [menginstal Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).

5. Setelah Office diinstal, ***jangan membuka atau masuk*** ke aplikasi Office apa pun.

6. Di RDS server, Aktifkan aktivasi komputer bersama dengan mengedit registri dengan mengikuti langkah berikut:

1. Klik kanan tombol Windows di sudut kiri bawah layar dan pilih Jalankan. Di kotak buka, ketik **regedit**, dan kemudian pilih OK.

2. Pilih Ya saat diminta untuk mengizinkan Penyunting registri untuk membuat perubahan pada perangkat Anda.

3. Di Penyunting registri, tambahkan nilai untai **Sharedcomputerlicensing** dengan pengaturan 1 di bawah HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Di RDS server, ***masuk sebagai pengguna akhir*** dan [verifikasi bahwa komputer bersama aktivasi diaktifkan untuk Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

Untuk rincian lebih lanjut tentang prasyarat, petunjuk penataan dan Panduan pada instalasi disesuaikan dengan menggunakan alat penyebaran Office, silakan lihat [menyebarkan office 365 ProPlus dengan menggunakan layanan desktop jarak jauh](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Untuk memperbaiki kesalahan yang terkait dengan aktivasi komputer bersama, silakan lihat [memecahkan masalah dengan aktivasi komputer bersama untuk Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  