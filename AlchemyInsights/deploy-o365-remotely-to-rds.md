---
title: Penyebaran Aplikasi Microsoft 365 untuk perusahaan untuk penggunaan bersama di RDS, Terminal Server, atau VDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 55b86557ec205dde2c459d76e8e330d2a8271dbec723f079e119ebe409b41c3f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031481"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Penyebaran Aplikasi Microsoft 365 untuk perusahaan untuk penggunaan bersama di RDS, Terminal Server, atau VDI

Untuk menyebarkan Aplikasi Microsoft 365 untuk perusahaan Layanan Desktop Jarak Jauh (RDS, Remote Desktop Services), yang sebelumnya bernama Terminal Services:

- Anda harus memiliki paket Microsoft 365 For Business atau paket Office 365 yang menyertakan Aplikasi Microsoft 365 untuk perusahaan, seperti Office 365 Enterprise E3 atau Enterprise E5.
   > [!NOTE]
   > Paket Aplikasi Microsoft 365 untuk bisnis dan Microsoft 365 Business Standard tersebut tidak menyertakan Aplikasi Microsoft 365 untuk perusahaan.
- Anda harus mengaktifkan [aktivasi komputer bersama](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> Anda juga dapat mengunduh dan menjalankan [Microsoft Asisten Dukungan dan Pemulihan](https://aka.ms/SaRA_OfficeSCA_M365Portal) menginstal Aplikasi Microsoft 365 untuk perusahaan mode aktivasi komputer bersama.

Untuk informasi selengkapnya tentang persyaratan, instruksi penyetelan, dan panduan tentang instalasi yang dikustomisasi dengan menggunakan Office Deployment Tool, lihat [Menyebarkan Aplikasi Microsoft 365 untuk perusahaan dengan menggunakan Layanan Desktop Jarak Jauh.](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)

Untuk memperbaiki kesalahan terkait aktivasi komputer bersama:

- Lihat [Memecahkan masalah dengan aktivasi komputer bersama untuk Aplikasi Microsoft 365 untuk perusahaan](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Lihat [Mengatur ulang status aktivasi Aplikasi Microsoft 365 untuk perusahaan](https://go.microsoft.com/fwlink/?linkid=2109218).

Jika Anda ingin menginstal Aplikasi Microsoft 365 untuk perusahaan di RDS dari pusat admin Microsoft 365, yang menggunakan pengaturan instalasi ***default,*** gunakan langkah-langkah berikut ini:

1. Periksa langganan apa yang Anda miliki. [Pelajari caranya.](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)
2. Jika perlu, beralihlah ke langganan lain. [Pelajari caranya.](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)
3. Jika Office sudah diinstal di server RDS menggunakan langganan Microsoft lainnya, hapus instalannya. Misalnya, dengan masuk ke **Panel Kontrol Hapus**  >  **instalan program**. Hapus [instalan menggunakan Microsoft Asisten Dukungan dan Pemulihan](https://aka.ms/SARA-OfficeUninstall-Alchemy) jika Anda mengalami masalah.
4. Di server RDS, masuk ke akun pusat admin Microsoft 365 akun administrator Anda dan instal [Aplikasi Microsoft 365 untuk perusahaan](https://portal.office.com/OLS/MySoftware.aspx).
5. Setelah Office diinstal, ***jangan buka atau masuk ke aplikasi*** Office pun.
6. Pada server RDS, aktifkan aktivasi komputer bersama dengan mengedit registri dengan mengikuti langkah-langkah ini:
   1. Klik kanan tombol Windows di sudut kiri bawah layar, lalu pilih **Jalankan**. Dalam kotak Buka, ketikkan **regedit**, lalu pilih **OK.**
   2. Pilih **Ya** ketika diminta untuk mengizinkan Editor Registri membuat perubahan pada perangkat Anda.
   3. Di Editor Registri, tambahkan nilai string **SharedComputerLicensing** dengan pengaturan 1 di bawah HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Pada server RDS, ***masuk sebagai pengguna akhir dan verifikasi*** bahwa aktivasi komputer bersama diaktifkan untuk [Aplikasi Microsoft 365 untuk perusahaan](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).
