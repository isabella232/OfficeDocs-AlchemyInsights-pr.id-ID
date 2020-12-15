---
title: Perangkat dalam status tertunda
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/11/2020
ms.locfileid: "49678483"
---
# <a name="device-in-pending-state"></a>Perangkat dalam status tertunda

**Tuntutan**

1. Jika Anda menyetel pendaftaran perangkat untuk pertama kalinya, pastikan bahwa Anda telah meninjau [pengenalan ke manajemen perangkat di Azure Active Directory (AZURE AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) yang akan memandu Anda tentang cara mendapatkan perangkat di bawah kontrol Azure AD.
2. Jika Anda mendaftarkan perangkat ke Azure AD secara langsung dan mendaftarkan mereka ke dalam Intune, Anda perlu memastikan bahwa Anda telah [mengonfigurasi Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) dan meminta [lisensi](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) tersebut terlebih dahulu.
3. Pastikan Anda memiliki wewenang untuk melakukan operasi di Azure AD dan AD di tempat. Hanya administrator global di Azure AD yang dapat mengelola pengaturan untuk pendaftaran perangkat. Selain itu, jika Anda menyetel pendaftaran otomatis di direktori aktif di tempat, Anda harus menjadi administrator direktori aktif dan AD FS (jika ada).

Proses registrasi gabungan Azure AD Pendaftaran memerlukan perangkat untuk berada di jaringan perusahaan. Ini juga berfungsi melalui VPN namun ada beberapa hal yang perlu diperhatikan. Kami telah mendengar Pelanggan yang memerlukan bantuan dengan pemecahan masalah hibrid Azure AD bergabung dalam proses pendaftaran di bawah kondisi kerja jarak jauh.

**Lingkungan autentikasi awan (menggunakan sinkronisasi hash kata sandi Azure atau autentikasi kirim langsung)**

Alur pendaftaran ini juga dikenal sebagai "gabungan sinkronisasi".

Berikut ini adalah rincian apa yang terjadi selama proses pendaftaran:

1. Windows 10 menemukan catatan koneksi Layanan (SCP) ketika pengguna masuk ke perangkat.

    1. Perangkat tersebut pertama kali mencoba untuk mengambil informasi penyewa dari SCP sisi klien dalam registri [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Untuk informasi selengkapnya, lihat [dokumen](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. Jika gagal, perangkat berkomunikasi dengan direktori aktif di tempat untuk mendapatkan informasi penyewa dari SCP. Untuk memverifikasi SCP, rujuk [dokumen](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)ini.

    > [!NOTE]
    > Kami merekomendasikan untuk mengaktifkan SCP di direktori aktif dan hanya menggunakan SCP sisi klien untuk validasi awal.

2. Windows 10 mencoba untuk berkomunikasi dengan Azure AD di bawah konteks sistem untuk mengautentikasi dirinya.

    Anda dapat memverifikasi apakah perangkat dapat mengakses sumber daya Microsoft di bawah akun sistem dengan menggunakan [skrip konektivitas registrasi perangkat uji](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).

3. Windows 10 menghasilkan sertifikat yang ditandatangani sendiri dan menyimpannya di bawah objek komputer di direktori aktif di tempat. Ini memerlukan garis pandang ke pengontrol domain.

4. Objek perangkat yang memiliki sertifikat disinkronkan ke Azure AD melalui Azure AD Connect. Siklus sinkronisasi adalah setiap 30 menit secara default, namun tergantung pada konfigurasi Azure AD Connect. Untuk informasi selengkapnya, lihat [dokumen](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)ini.

5. Pada tahap ini, Anda akan bisa melihat perangkat subjek dalam status "**tertunda**" di bawah bilah perangkat Azure portal.

6. Di pengguna berikutnya masuk ke Windows 10, pendaftaran akan diselesaikan.

    > [!NOTE]
    > Jika Anda berada di VPN dan logoff/login mengakhiri konektivitas domain, Anda bisa memicu pendaftaran secara manual. Untuk melakukan itu:
    >
    > Masalah `dsregcmd /join` secara lokal pada prompt admin atau jarak jauh melalui PSExec ke PC Anda.
    >
    > Misalnya: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Untuk masalah umum dengan pendaftaran perangkat Azure Active Directory, lihat [FAQ perangkat](https://docs.microsoft.com/azure/active-directory/devices/faq).
