---
title: Menyebarkan Office 365 ProPlus untuk digunakan bersama di RDS, terminal server, atau VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959463"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a>Menyebarkan Office 365 ProPlus untuk digunakan bersama di RDS, terminal server, atau VDI

Untuk menyebarkan Office 365 ProPlus menggunakan layanan desktop jarak jauh (RDS), sebelumnya bernama Layanan Terminal:
- Anda harus memiliki Microsoft 365 untuk rencana bisnis atau Office 365 rencana yang mencakup Office 365 ProPlus, seperti Office 365 Enterprise E3 atau Enterprise E5.
   > [!NOTE] 
   > Office 365 bisnis dan Office 365 rencana bisnis Premium tidak termasuk Office 365 ProPlus.
- Anda harus mengaktifkan [aktivasi komputer bersama](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

> [!NOTE]
> Anda juga dapat mengunduh dan menjalankan [dukungan Microsoft dan asisten pemulihan](https://aka.ms/SaRA_OfficeSCA_M365Portal) untuk menginstal Office 365 ProPlus dalam mode aktivasi komputer bersama.

Untuk informasi lebih lanjut tentang prasyarat, petunjuk penataan, dan Panduan pada instalasi disesuaikan dengan menggunakan alat penyebaran Office, lihat [menyebarkan office 365 ProPlus dengan menggunakan layanan desktop jarak jauh](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).

Untuk memperbaiki kesalahan yang terkait dengan aktivasi komputer bersama:
- Lihat [memecahkan masalah dengan aktivasi komputer bersama untuk Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
- Lihat [reset Office 365 ProPlus aktivasi negara](https://go.microsoft.com/fwlink/?linkid=2109218).

Jika Anda ingin menginstal Office 365 ProPlus di RDS dari Microsoft 365 Admin Center, ***yang menggunakan pengaturan instalasi default***, gunakan langkah-langkah berikut ini:

1.  Periksa apa Office 365 rencana yang Anda miliki. [Pelajari caranya](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).
2.  Jika perlu, beralih ke rencana Office 365 yang berbeda. [Pelajari caranya](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).
3.  Jika Office sudah diinstal di RDS server menggunakan rencana Office 365 lainnya, bongkar. Misalnya, dengan pergi ke **Control Panel** > **Uninstall program**. Membongkar menggunakan [dukungan Microsoft dan pemulihan asisten](https://aka.ms/SARA-OfficeUninstall-Alchemy) jika Anda menjalankan ke masalah.
4.  Di RDS server, masuk ke Microsoft 365 Admin Center dengan akun administrator dan [menginstal Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).
5.  Setelah Office diinstal, ***jangan membuka atau masuk*** ke aplikasi Office apa pun.
6.  Di RDS server, Aktifkan aktivasi komputer bersama dengan mengedit registri dengan mengikuti langkah berikut:
   1. Klik kanan tombol Windows di sudut kiri bawah layar Anda dan pilih **Jalankan**. Di kotak buka, ketik **regedit**, dan kemudian pilih **OK**.
   2. Pilih **ya** saat diminta untuk mengizinkan Penyunting registri untuk membuat perubahan pada perangkat Anda.
   3. Di Penyunting registri, tambahkan nilai untai **Sharedcomputerlicensing** dengan pengaturan 1 di bawah HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Di RDS server, ***masuk sebagai pengguna akhir*** dan [verifikasi bahwa komputer bersama aktivasi diaktifkan untuk Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

