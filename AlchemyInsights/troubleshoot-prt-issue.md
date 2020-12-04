---
title: Memecahkan masalah PRT
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573718"
---
# <a name="troubleshoot-prt-issue"></a>Memecahkan masalah PRT

Untuk perangkat apa pun yang diselesaikan dengan benar, harus terdaftar dan di negara bagian yang baik dan dapat memperoleh token refresh utama (PRT).

Proses registrasi gabungan Azure AD Pendaftaran memerlukan perangkat untuk berada di jaringan perusahaan. Ini juga berfungsi melalui VPN namun ada beberapa hal yang perlu diperhatikan. Kami telah mendengar Pelanggan yang memerlukan bantuan dengan pemecahan masalah hibrid proses pendaftaran gabungan Azure AD di bawah kondisi kerja jarak jauh. Berikut ini adalah rincian apa yang terjadi ' di bawah kap ' selama proses registrasi.

**Lingkungan autentikasi awan (menggunakan sinkronisasi hash kata sandi Azure atau autentikasi kirim langsung)**

Alur pendaftaran ini juga dikenal sebagai "gabungan sinkronisasi".

1. Windows 10 menemukan catatan SCP saat pengguna masuk ke perangkat.
    1. Perangkat tersebut pertama kali mencoba untuk mengambil informasi penyewa dari SCP sisi klien dalam registri [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Untuk informasi selengkapnya, lihat [dokumen](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)ini.
    2. Jika gagal, perangkat berkomunikasi dengan Active Directory lokal (AD) untuk mendapatkan informasi penyewa dari titik koneksi Layanan (SCP). Untuk memverifikasi SCP, silakan lihat [dokumen](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)ini. 

> [!NOTE]
> Kami merekomendasikan untuk mengaktifkan SCP dalam iklan dan hanya menggunakan SCP sisi klien untuk validasi awal.

2. Windows 10 mencoba untuk berkomunikasi dengan Azure AD di bawah konteks sistem untuk mengautentikasi dirinya. Anda dapat memverifikasi apakah perangkat dapat mengakses sumber daya Microsoft di bawah akun sistem dengan menggunakan skrip konektivitas registrasi perangkat uji.

3. Windows 10 menghasilkan sertifikat yang ditandatangani sendiri dan menyimpannya di bawah objek komputer di AD di tempat. Ini memerlukan garis pandang ke pengontrol domain.

4. Objek perangkat yang memiliki sertifikat disinkronkan ke Azure AD melalui Azure AD Connect. Siklus sinkronisasi adalah setiap 30 menit secara default, namun tergantung pada konfigurasi Azure AD Connect. Untuk informasi selengkapnya, lihat [dokumen](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)ini.

5. Pada tahap ini, Anda akan bisa melihat perangkat subjek dalam status "tertunda" di bawah bilah perangkat Azure portal.

6. Di pengguna berikutnya masuk ke Windows 10, pendaftaran akan diselesaikan. 

> [!NOTE]
> Jika Anda menggunakan VPN dan logoff-proses masuk mengakhiri konektivitas domain, Anda bisa memicu pendaftaran secara manual:
 1. Menerbitkan dsregcmd/Join secara lokal pada prompt admin atau jarak jauh melalui PSExec ke PC Anda. Sebagai contoh, PsExec-s \\ win10client01 CMD, dsregcmd/Join

 2. Untuk detail selengkapnya tentang masalah gabungan hibrid, lihat [memecahkan masalah perangkat](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).
