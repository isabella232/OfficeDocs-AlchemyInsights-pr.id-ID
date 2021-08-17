---
title: Menginstal office di Terminal Server - Tidak Memiliki Lisensi
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 7e435df1515878ab4fe935ab8148daee29b8e3820095fc6e49db45de4c6279db
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055161"
---
# <a name="installing-office-on-a-terminal-server"></a>Menginstal Office di Terminal Server

Untuk menyebarkan Aplikasi Microsoft 365 untuk perusahaan server Windows menggunakan Remote Desktop Services (RDS), yang sebelumnya bernama Terminal Services:
  
- Anda harus memiliki langganan Microsoft 365 yang menyertakan Aplikasi Microsoft 365 untuk perusahaan, seperti Office 365 Enterprise E3 atau Enterprise E5. Paket Aplikasi Microsoft 365 untuk bisnis dan Aplikasi Microsoft 365 untuk bisnis Premium paket tersebut tidak menyertakan Aplikasi Microsoft 365 untuk perusahaan.

- Anda perlu mengaktifkan [aktivasi komputer bersama](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Jika Anda ingin menginstal Aplikasi Microsoft 365 untuk perusahaan di RDS dari pusat admin Microsoft 365, yang menggunakan pengaturan instalasi ***default,*** gunakan langkah-langkah berikut ini.

> [!TIP]
> Anda juga dapat mengunduh dan menjalankan [Microsoft Asisten Dukungan dan Pemulihan](https://aka.ms/SaRA_OfficeSCA_M365Portal) menginstal Aplikasi Microsoft 365 untuk perusahaan mode aktivasi komputer bersama.
  
1. Periksa langganan Microsoft 365 apa yang Anda miliki. [Pelajari caranya](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Jika perlu, beralihlah ke langganan Microsoft 365 lain. [Pelajari caranya](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Jika Office sudah diinstal di server RDS menggunakan langganan lain Microsoft 365, hapus instalannya. Misalnya, dengan masuk ke Panel Kontrol \> Hapus instalan program. Hapus [instalan menggunakan Microsoft Asisten Dukungan dan Pemulihan](https://aka.ms/SARA-OfficeUninstall-Alchemy) jika Anda mengalami masalah.

4. Di server RDS, masuk ke akun pusat admin Microsoft 365 akun administrator Anda dan instal [Aplikasi Microsoft 365 untuk perusahaan](https://portal.office.com/OLS/MySoftware.aspx).

5. Setelah Office diinstal, ***jangan buka atau masuk ke aplikasi*** Office pun.

6. Pada server RDS, aktifkan aktivasi komputer bersama dengan mengedit registri dengan mengikuti langkah-langkah ini:

1. Klik kanan Windows di sudut kiri bawah layar, lalu pilih Jalankan. Dalam kotak Buka, ketikkan **regedit**, lalu pilih OK.

2. Pilih Ya ketika diminta untuk mengizinkan Editor Registri membuat perubahan pada perangkat Anda.

3. Di Editor Registri, tambahkan nilai string **SharedComputerLicensing** dengan pengaturan 1 di bawah HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Pada server RDS, ***masuk sebagai pengguna akhir dan verifikasi*** bahwa aktivasi komputer bersama diaktifkan untuk [Aplikasi Microsoft 365 untuk perusahaan](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Untuk detail selengkapnya tentang persyaratan, instruksi penyetelan, dan panduan tentang instalasi yang dikustomisasi dengan menggunakan Office Deployment Tool, silakan lihat Menyebarkan Aplikasi Microsoft 365 untuk perusahaan dengan menggunakan [Layanan Desktop Jarak Jauh.](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)
  
Untuk memperbaiki kesalahan terkait aktivasi komputer bersama, silakan lihat [Memecahkan masalah dengan aktivasi komputer bersama untuk Aplikasi Microsoft 365 untuk perusahaan](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  