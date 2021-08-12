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
ms.openlocfilehash: 224e6e613c306b50e354930bcbe6f43f1c08528766cb6e681b0e9826b2d55a4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914006"
---
# <a name="device-in-pending-state"></a>Perangkat dalam status tertunda

**Prasyarat:**

1. Jika Anda menyiapkan pendaftaran perangkat untuk kali pertama, pastikan Anda telah meninjau Pengenalan pada manajemen perangkat di [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) yang akan memandu Anda tentang cara mendapatkan perangkat di bawah kontrol Azure AD.
2. Jika mendaftarkan perangkat ke Azure AD secara langsung dan mendaftarkan perangkat ke Intune, Pastikan Anda telah mengonfigurasi [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) dan lisensinya tersedia terlebih dahulu.
3. Pastikan Anda memiliki wewenang untuk melakukan operasi di Azure AD dan AD lokal. Hanya administrator global di Microsoft Azure AD yang dapat mengelola pengaturan untuk pendaftaran perangkat. Selain itu, jika Anda menyiapkan pendaftaran otomatis di Active Directory lokal, Anda perlu menjadi administrator Active Directory dan AD FS (jika berlaku).

Proses pendaftaran gabungan Azure AD hibrid memerlukan perangkat untuk berada di jaringan perusahaan. Peringatan juga dapat digunakan di VPN, tetapi terdapat beberapa peringatan untuk hal tersebut. Kami telah mendengar pelanggan yang membutuhkan bantuan dalam pemecahan masalah proses pendaftaran gabungan Azure AD hibrid dalam keadaan kerja jarak jauh.

**Lingkungan autentikasi cloud (menggunakan sinkronisasi hash kata sandi Azure AD atau autentikasi langsung)**

Aliran pendaftaran ini juga dikenal sebagai "Sinkronisasi Gabung".

Berikut uraian dari apa yang terjadi selama pendaftaran:

1. Windows 10 menemukan catatan Service Connection Point (SCP) saat pengguna masuk ke perangkat.

    1. Perangkat pertama mencoba mengambil informasi penyewa dari SCP pihak klien dalam registri [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Untuk informasi selengkapnya, lihat [dokumen](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. Jika gagal, perangkat berkomunikasi dengan Direktori Aktif di tempat untuk mendapatkan informasi penyewa dari SCP. Untuk memverifikasi SCP, rujuk dokumen [ini.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)

    > [!NOTE]
    > Kami menyarankan mengaktifkan SCP di Direktori Aktif dan hanya menggunakan SCP pihak klien untuk validasi awal.

2. Windows 10 mencoba berkomunikasi dengan Azure AD di bawah konteks sistem untuk mengautentikasi dirinya terhadap Azure AD.

    Anda bisa memverifikasi apakah perangkat bisa mengakses sumber daya Microsoft di bawah akun sistem dengan menggunakan [skrip Konektivitas Registrasi Perangkat Uji.](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0)

3. Windows 10 menghasilkan sertifikat yang ditandatangani sendiri dan menyimpannya di bawah objek komputer di Direktori Aktif lokal. Hal ini membutuhkan pengontrol domain yang tak terlihat.

4. Objek perangkat yang memiliki sertifikat disinkronkan ke Azure AD melalui Azure AD Koneksi. Siklus sinkronisasi adalah setiap 30 menit secara default, tetapi bergantung pada konfigurasi Azure AD Koneksi. Untuk informasi selengkapnya, lihat dokumen [ini.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. Pada tahap ini, Anda akan dapat melihat perangkat subjek dalam status "**Tertunda**" di bawah Blade perangkat Portal Azure.

6. Pada pengguna berikutnya masuk Windows 10, pendaftaran akan diselesaikan.

    > [!NOTE]
    > Jika Anda berada di VPN dan logoff/login mengakhiri konektivitas domain, Anda dapat memicu pendaftaran secara manual. Untuk melakukannya:
    >
    > Masalah lokal `dsregcmd /join` pada perintah admin atau secara jarak jauh melalui PSExec ke PC Anda.
    >
    > Misalnya: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Untuk masalah umum terkait pendaftaran Azure Active Directory, lihat [FAQ Perangkat.](https://docs.microsoft.com/azure/active-directory/devices/faq)
