---
title: Menginstal Office di terminal server-tanpa lisensi
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
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663120"
---
# <a name="installing-office-on-a-terminal-server"></a>Menginstal Office di server terminal

Untuk menyebarkan aplikasi Microsoft 365 untuk perusahaan di server Windows menggunakan layanan desktop jarak jauh (RDS), sebelumnya bernama Layanan Terminal:
  
- Anda harus memiliki langganan Microsoft 365 yang menyertakan aplikasi Microsoft 365 untuk perusahaan, seperti Office 365 Enterprise E3 atau Enterprise E5. Paket aplikasi Microsoft 365 untuk bisnis dan Microsoft 365 aplikasi untuk bisnis Premium tidak menyertakan aplikasi Microsoft 365 untuk perusahaan.

- Anda perlu mengaktifkan [aktivasi komputer bersama](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Jika Anda ingin menginstal aplikasi Microsoft 365 untuk perusahaan di RDS dari Pusat admin Microsoft 365, ***yang menggunakan pengaturan instalasi default***, gunakan langkah-langkah berikut ini.

> [!TIP]
> Anda juga bisa mengunduh dan menjalankan [asisten dukungan dan pemulihan Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) untuk menginstal aplikasi Microsoft 365 untuk perusahaan dalam mode aktivasi komputer bersama.
  
1. Lihat langganan Microsoft 365 apa yang Anda miliki. [Pelajari caranya](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Jika perlu, alihkan ke langganan Microsoft 365 yang berbeda. [Pelajari caranya](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Jika Office telah terinstal di server RDS menggunakan langganan Microsoft 365 lainnya, Hapus instalasinya. Misalnya, dengan masuk ke panel kontrol \> hapus instalan program. Hapus instalan menggunakan [asisten dukungan dan pemulihan Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) jika Anda mengalami masalah.

4. Di server RDS, masuk ke Pusat admin Microsoft 365 dengan akun administrator Anda dan [instal aplikasi Microsoft 365 untuk perusahaan](https://portal.office.com/OLS/MySoftware.aspx).

5. Setelah Office terinstal, ***jangan buka atau masuk*** ke aplikasi Office apa pun.

6. Di server RDS, Aktifkan aktivasi komputer bersama dengan mengedit registri dengan mengikuti langkah berikut:

1. Klik kanan tombol Windows di sudut kiri bawah layar Anda, lalu pilih Jalankan. Dalam kotak buka, ketikkan **regedit**, lalu pilih OK.

2. Pilih Ya ketika diminta untuk memperbolehkan editor registri untuk membuat perubahan pada perangkat Anda.

3. Dalam editor registri, tambahkan nilai string **Sharedcomputerlicensing** dengan pengaturan 1 di bawah HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Di server RDS, ***masuk sebagai pengguna akhir*** dan [verifikasi bahwa aktivasi komputer bersama diaktifkan untuk aplikasi Microsoft 365 untuk perusahaan](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Untuk detail selengkapnya tentang prasyarat, instruksi penyetelan dan panduan tentang instalasi yang dikustomisasi dengan menggunakan alat penyebaran Office, silakan lihat [menyebarkan aplikasi Microsoft 365 untuk perusahaan dengan menggunakan layanan desktop jarak jauh](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Untuk memperbaiki kesalahan terkait aktivasi komputer bersama, silakan lihat [memecahkan masalah dengan aktivasi komputer bersama untuk aplikasi Microsoft 365 untuk perusahaan](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  