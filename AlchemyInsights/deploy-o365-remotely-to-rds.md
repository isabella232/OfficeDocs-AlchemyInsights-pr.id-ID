---
title: Penyebaran Aplikasi Microsoft 365 untuk penggunaan bersama di RDS, Terminal Server, atau VDI
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
ms.openlocfilehash: 81183cf1823480c1b15eba9ba9f519b4e3746b52
ms.sourcegitcommit: ef8d6b71fbd962fb3f7081b21724e67a91111a92
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/01/2021
ms.locfileid: "60077253"
---
# <a name="deploying-microsoft-365-apps-for-shared-use-on-rds-terminal-server-or-vdi"></a>Penyebaran Aplikasi Microsoft 365 untuk penggunaan bersama di RDS, Terminal Server, atau VDI

Untuk menyebarkan Aplikasi Microsoft 365 Remote Desktop Services (RDS), sebelumnya Terminal Services, Anda harus:

- Gunakan perbaikan mudah untuk mengaktifkan TLS 1.2 sebagai default jika Anda menjalankan versi Windows yang lebih lama (misalnya Windows 7 SP1, Windows Server 2008 R2). Untuk perbaikan mudah dan informasi selengkapnya, lihat Pembaruan untuk mengaktifkan [TLS 1.1 dan TLS 1.2](https://support.microsoft.com/en-us/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392#bkmk_easy)sebagai protokol aman default di WinHTTP di Windows . 
- Memiliki paket yang menyertakan Aplikasi Microsoft 365 untuk perusahaan (sebelumnya Office 365 Plus). Misalnya, Office 365 E3 atau Microsoft 365 E5, atau paket apa pun yang menyertakan Visio atau Project versi desktop, seperti Project Paket 3 atau Visio Paket 2, atau paket Microsoft 365 Business Premium, yang juga menyertakan Aplikasi Microsoft 365 untuk bisnis.
- Mengaktifkan aktivasi komputer bersama. Untuk informasi selengkapnya, lihat [Gambaran umum aktivasi komputer bersama untuk Aplikasi Microsoft 365](https://docs.microsoft.com/deployoffice/overview-shared-computer-activation).

**Catatan**: Untuk menginstal Aplikasi Microsoft 365 dalam mode aktivasi komputer bersama, unduh dan jalankan [Microsoft Asisten Dukungan dan Pemulihan](https://aka.ms/SaRA_OfficeSCA_M365Portal). Untuk detail tentang persyaratan, instruksi penyetelan, dan panduan untuk mengkustomisasi instalasi dengan menggunakan Office Deployment Tool, lihat Menyebarkan Aplikasi Microsoft 365 dengan menggunakan [Layanan Desktop Jarak Jauh.](https://docs.microsoft.com/deployoffice/deploy-microsoft-365-apps-remote-desktop-services)

Untuk memperbaiki kesalahan terkait aktivasi komputer bersama, lihat:

- [Memecahkan masalah dengan aktivasi komputer bersama untuk Aplikasi Microsoft 365](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation)
- [Mereset Aplikasi Microsoft 365 untuk perusahaan status aktivasi](https://docs.microsoft.com/office/troubleshoot/activation/reset-office-365-proplus-activation-state)

Jika Anda ingin menginstal Aplikasi Microsoft 365 di RDS dari pusat admin Microsoft 365, yang menggunakan pengaturan instalasi default, ikuti langkah-langkah ini:

1. Periksa paket Microsoft 365 apa yang Anda miliki. Untuk informasi selengkapnya, lihat [Langganan apa yang saya miliki?](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).

1. Jika perlu, beralihlah ke paket Microsoft 365 lain. Untuk informasi selengkapnya, lihat [Memutakhirkan ke paket lain.](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan)

1. Jika Aplikasi Microsoft 365 sudah diinstal di server RDS menggunakan paket tidak kompatibel lainnya, hapus instalasinya dengan masuk ke **Panel** Kontrol Hapus instalasi  >  **program**. Jika Anda mengalami masalah, hapus instalasi dengan mengunduh [Microsoft Asisten Dukungan dan Pemulihan](https://aka.ms/SARA-OfficeUninstall-Alchemy).

1. Di server RDS, masuk ke akun pusat admin Microsoft 365 akun administrator Anda dan instal [Office](https://portal.office.com/OLS/MySoftware.aspx).

   Setelah Office diinstal, jangan buka atau masuk ke aplikasi Office apa pun.

1. Pada server RDS, aktifkan aktivasi komputer bersama dengan mengedit registri:

   1. Klik kanan Windows di sudut kiri bawah layar, lalu pilih **Jalankan**. Dalam kotak Buka, ketikkan **regedit**, lalu pilih **OK.**

   1. Ketika diminta untuk mengizinkan Editor Registri membuat perubahan ke perangkat Anda, pilih **Ya**.

   1. Di Editor Registri, di bawah HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration, tambahkan nilai string **SharedComputerLicensing** dengan pengaturan **1** .

1. Pada server RDS, masuk sebagai pengguna akhir dan verifikasi bahwa aktivasi komputer bersama diaktifkan untuk Aplikasi Microsoft 365. 

   Untuk detailnya, [lihat Memverifikasi bahwa aktivasi komputer bersama diaktifkan untuk Aplikasi Microsoft 365](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation#verify-that-shared-computer-activation-is-enabled-for-microsoft-365-apps).