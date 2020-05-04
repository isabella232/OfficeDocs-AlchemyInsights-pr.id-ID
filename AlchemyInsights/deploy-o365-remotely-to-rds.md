---
title: Menyebarkan Microsoft 365 Apps untuk perusahaan untuk digunakan bersama di RDS, terminal server, atau VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 51512b29f8d37ce6c39ece5bb704cb01e88e463d
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010257"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Menyebarkan Microsoft 365 Apps untuk perusahaan untuk digunakan bersama di RDS, terminal server, atau VDI

Untuk menyebarkan Microsoft 365 aplikasi untuk perusahaan yang menggunakan layanan desktop jarak jauh (RDS), sebelumnya bernama Layanan Terminal:
- Anda harus memiliki Microsoft 365 untuk rencana bisnis atau Office 365 rencana yang mencakup Microsoft 365 aplikasi untuk perusahaan, seperti Office 365 Enterprise E3 atau Enterprise E5.
   > [!NOTE] 
   > Microsoft 365 aplikasi untuk bisnis dan Microsoft 365 bisnis Premium standar rencana tidak termasuk Microsoft 365 aplikasi untuk perusahaan.
- Anda harus mengaktifkan [aktivasi komputer bersama](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> Anda juga dapat mengunduh dan menjalankan [dukungan Microsoft dan asisten pemulihan](https://aka.ms/SaRA_OfficeSCA_M365Portal) untuk menginstal Microsoft 365 aplikasi untuk perusahaan dalam mode aktivasi komputer bersama.

Untuk informasi lebih lanjut tentang prasyarat, petunjuk penataan, dan Panduan pada instalasi disesuaikan dengan menggunakan alat penyebaran Office, lihat [menyebarkan Microsoft 365 aplikasi untuk perusahaan dengan menggunakan layanan desktop jarak jauh](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

Untuk memperbaiki kesalahan yang terkait dengan aktivasi komputer bersama:
- Lihat [memecahkan masalah dengan aktivasi komputer bersama untuk Microsoft 365 aplikasi untuk perusahaan](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Lihat [Mengatur ulang status aktivasi Aplikasi Microsoft 365 untuk perusahaan](https://go.microsoft.com/fwlink/?linkid=2109218).

Jika Anda ingin menginstal Microsoft 365 aplikasi untuk perusahaan di RDS dari Microsoft 365 Admin Center, ***yang menggunakan pengaturan instalasi default***, gunakan langkah-langkah berikut ini:

1.    Periksa langganan apa yang Anda miliki. [Pelajari caranya](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).
2.    Jika perlu, beralih ke langganan yang berbeda. [Pelajari caranya](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).
3.    Jika Office sudah diinstal di RDS server menggunakan langganan Microsoft lainnya, bongkar. Misalnya, dengan pergi ke **Control Panel** > **Uninstall program**. Membongkar menggunakan [dukungan Microsoft dan pemulihan asisten](https://aka.ms/SARA-OfficeUninstall-Alchemy) jika Anda menjalankan ke masalah.
4.    Di RDS server, masuk ke Pusat admin Microsoft 365 dengan akun administrator dan [menginstal microsoft 365 aplikasi untuk perusahaan](https://portal.office.com/OLS/MySoftware.aspx).
5.    Setelah Office diinstal, ***jangan membuka atau masuk*** ke aplikasi Office apa pun.
6.    Di RDS server, Aktifkan aktivasi komputer bersama dengan mengedit registri dengan mengikuti langkah berikut:
   1. Klik kanan tombol Windows di sudut kiri bawah layar Anda dan pilih **Jalankan**. Di kotak buka, ketik **regedit**, dan kemudian pilih **OK**.
   2. Pilih **ya** saat diminta untuk mengizinkan Penyunting registri untuk membuat perubahan pada perangkat Anda.
   3. Di Penyunting registri, tambahkan nilai untai **Sharedcomputerlicensing** dengan pengaturan 1 di bawah HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Di RDS server, ***masuk sebagai pengguna akhir*** dan [verifikasi bahwa komputer bersama aktivasi diaktifkan untuk Microsoft 365 aplikasi untuk perusahaan](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

