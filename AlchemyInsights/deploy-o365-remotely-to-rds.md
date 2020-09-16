---
title: Menyebarkan aplikasi Microsoft 365 untuk perusahaan untuk penggunaan bersama di RDS, terminal server, atau VDI
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 22ded616e82b2e82023b55a1d3ca6251cfb71712
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745538"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Menyebarkan aplikasi Microsoft 365 untuk perusahaan untuk penggunaan bersama di RDS, terminal server, atau VDI

Untuk menggunakan aplikasi Microsoft 365 untuk perusahaan dengan Remote Desktop Services (RDS), sebelumnya bernama Services terminal:
- Anda harus memiliki paket Microsoft 365 for Business atau paket Office 365 yang menyertakan aplikasi Microsoft 365 untuk perusahaan, seperti Office 365 Enterprise E3 atau Enterprise E5.
   > [!NOTE] 
   > Paket aplikasi Microsoft 365 for Business dan Microsoft 365 Business Premium Premium tidak menyertakan aplikasi Microsoft 365 untuk perusahaan.
- Anda harus mengaktifkan [aktivasi komputer bersama](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> Anda juga bisa mengunduh dan menjalankan [asisten dukungan dan pemulihan Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) untuk menginstal aplikasi Microsoft 365 untuk perusahaan dalam mode aktivasi komputer bersama.

Untuk informasi selengkapnya tentang prasyarat, instruksi penyetelan, dan panduan tentang instalasi yang dikustomisasi dengan menggunakan alat penyebaran Office, lihat [menyebarkan aplikasi Microsoft 365 untuk perusahaan dengan menggunakan layanan desktop jarak jauh](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

Untuk memperbaiki kesalahan terkait aktivasi komputer bersama:
- Lihat [memecahkan masalah dengan aktivasi komputer bersama untuk aplikasi Microsoft 365 untuk perusahaan](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Lihat [Mengatur ulang status aktivasi Aplikasi Microsoft 365 untuk perusahaan](https://go.microsoft.com/fwlink/?linkid=2109218).

Jika Anda ingin menginstal aplikasi Microsoft 365 untuk perusahaan di RDS dari Pusat admin Microsoft 365, ***yang menggunakan pengaturan instalasi default***, gunakan langkah-langkah berikut ini:

1.    Periksa langganan yang Anda miliki. [Pelajari caranya](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2.    Jika perlu, alihkan ke langganan lain. [Pelajari caranya](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3.    Jika Office telah terinstal di server RDS menggunakan langganan Microsoft lainnya, hapus instalan. Misalnya, dengan masuk ke **panel kontrol**  >  **hapus instalan program**. Hapus instalan menggunakan [asisten dukungan dan pemulihan Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) jika Anda mengalami masalah.
4.    Di server RDS, masuk ke Pusat admin Microsoft 365 dengan akun administrator Anda dan [instal aplikasi Microsoft 365 untuk perusahaan](https://portal.office.com/OLS/MySoftware.aspx).
5.    Setelah Office terinstal, ***jangan buka atau masuk*** ke aplikasi Office apa pun.
6.    Di server RDS, Aktifkan aktivasi komputer bersama dengan mengedit registri dengan mengikuti langkah berikut:
   1. Klik kanan tombol Windows di sudut kiri bawah layar Anda, lalu pilih **Jalankan**. Dalam kotak buka, ketikkan **regedit**, lalu pilih **OK**.
   2. Pilih **ya** ketika diminta untuk memperbolehkan editor registri untuk membuat perubahan pada perangkat Anda.
   3. Dalam editor registri, tambahkan nilai string **Sharedcomputerlicensing** dengan pengaturan 1 di bawah HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Di server RDS, ***masuk sebagai pengguna akhir*** dan [verifikasi bahwa aktivasi komputer bersama diaktifkan untuk aplikasi Microsoft 365 untuk perusahaan](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

