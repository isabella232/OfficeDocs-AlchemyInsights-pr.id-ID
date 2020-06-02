---
title: Menginstal Office di terminal server-tidak berlisensi
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: c781e9fd492ff97bc80667956e6609b3d40b28b4
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508631"
---
# <a name="installing-office-on-a-terminal-server"></a>Menginstal Office di terminal server

Untuk menyebarkan Microsoft 365 aplikasi untuk perusahaan di Windows Server menggunakan layanan desktop jarak jauh (RDS), sebelumnya bernama Layanan Terminal:
  
- Anda harus memiliki langganan Microsoft 365 yang mencakup Microsoft 365 aplikasi untuk perusahaan, seperti Office 365 Enterprise E3 atau Enterprise E5. Microsoft 365 aplikasi untuk bisnis dan Microsoft 365 aplikasi untuk bisnis Premium rencana tidak termasuk Microsoft 365 aplikasi untuk perusahaan.

- Anda harus mengaktifkan [aktivasi komputer bersama](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Jika Anda ingin menginstal Microsoft 365 aplikasi untuk perusahaan di RDS dari Microsoft 365 Admin Center, ***yang menggunakan pengaturan instalasi default***, gunakan langkah-langkah berikut ini.

> [!TIP]
> Anda juga dapat mengunduh dan menjalankan [dukungan Microsoft dan asisten pemulihan](https://aka.ms/SaRA_OfficeSCA_M365Portal) untuk menginstal Microsoft 365 aplikasi untuk perusahaan dalam mode aktivasi komputer bersama.
  
1. Periksa apa langganan Microsoft 365 yang Anda miliki. [Pelajari caranya](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Jika perlu, beralih ke langganan Microsoft 365 yang berbeda. [Pelajari caranya](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Jika Office sudah diinstal di RDS server menggunakan langganan Microsoft 365 lainnya, uninstall. Sebagai contoh, dengan pergi ke Control Panel \> Uninstall program. Membongkar menggunakan [dukungan Microsoft dan pemulihan asisten](https://aka.ms/SARA-OfficeUninstall-Alchemy) jika Anda menjalankan ke masalah.

4. Di RDS server, masuk ke Pusat admin Microsoft 365 dengan akun administrator dan [menginstal microsoft 365 aplikasi untuk perusahaan](https://portal.office.com/OLS/MySoftware.aspx).

5. Setelah Office diinstal, ***jangan membuka atau masuk*** ke aplikasi Office apa pun.

6. Di RDS server, Aktifkan aktivasi komputer bersama dengan mengedit registri dengan mengikuti langkah berikut:

1. Klik kanan tombol Windows di sudut kiri bawah layar dan pilih Jalankan. Di kotak buka, ketik **regedit**, dan kemudian pilih OK.

2. Pilih Ya saat diminta untuk mengizinkan Penyunting registri untuk membuat perubahan pada perangkat Anda.

3. Di Penyunting registri, tambahkan nilai untai **Sharedcomputerlicensing** dengan pengaturan 1 di bawah HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Di RDS server, ***masuk sebagai pengguna akhir*** dan [verifikasi bahwa komputer bersama aktivasi diaktifkan untuk Microsoft 365 aplikasi untuk perusahaan](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Untuk rincian lebih lanjut tentang prasyarat, petunjuk penataan dan Panduan pada instalasi disesuaikan dengan menggunakan alat penyebaran Office, silakan lihat [menyebarkan Microsoft 365 aplikasi untuk perusahaan dengan menggunakan layanan desktop jarak jauh](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Untuk memperbaiki kesalahan yang terkait dengan aktivasi komputer bersama, silakan lihat [memecahkan masalah dengan aktivasi komputer bersama untuk Microsoft 365 aplikasi untuk perusahaan](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  