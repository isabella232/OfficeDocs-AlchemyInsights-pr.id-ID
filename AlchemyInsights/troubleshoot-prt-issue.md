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
ms.openlocfilehash: a005c4a6848bbf0725560375df1220ce906cbb5f
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330962"
---
# <a name="troubleshoot-prt-issue"></a>Memecahkan masalah PRT

Agar perangkat apa pun dapat menyelesaikan autentikasi, perangkat harus terdaftar sepenuhnya dan dalam keadaan baik serta dapat memperoleh Token Refresh Utama (PRT).

Proses pendaftaran gabungan Azure AD hibrid memerlukan perangkat untuk berada di jaringan perusahaan. Peringatan juga dapat digunakan di VPN, tetapi terdapat beberapa peringatan untuk hal tersebut. Kami telah mendengar pelanggan yang membutuhkan bantuan dalam pemecahan masalah proses pendaftaran gabungan Azure AD hibrid dalam keadaan kerja jarak jauh. Berikut uraian tentang apa yang terjadi 'di balik balik layar' selama proses pendaftaran.

**Lingkungan autentikasi cloud (menggunakan sinkronisasi hash kata sandi Azure AD atau autentikasi langsung)**

Aliran pendaftaran ini juga dikenal sebagai "Sinkronisasi Gabung".

1. Windows 10 menemukan catatan SCP pada saat pengguna masuk ke perangkat.
    1. Perangkat pertama mencoba mengambil informasi penyewa dari SCP pihak klien dalam registri [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Untuk informasi selengkapnya, lihat dokumen [ini](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    2. Jika gagal, perangkat berkomunikasi dengan Direktori Aktif (AD) di tempat untuk mendapatkan informasi penyewa dari Service Connection Point (SCP). Untuk memverifikasi SCP, silakan rujuk ke dokumen [ini.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point) 

**Catatan**: Kami menyarankan untuk mengaktifkan SCP di AD dan hanya menggunakan SCP pihak klien untuk validasi awal.

2. Windows 10 mencoba berkomunikasi dengan Azure AD di bawah konteks sistem untuk mengautentikasi dirinya terhadap Azure AD. Anda bisa memverifikasi apakah perangkat bisa mengakses sumber daya Microsoft di bawah akun sistem dengan menggunakan skrip Konektivitas Registrasi Perangkat Uji.

3. Windows 10 akan menghasilkan sertifikat yang ditandatangani sendiri dan menyimpannya di bawah objek komputer di AD lokal. Hal ini membutuhkan pengontrol domain yang tak terlihat.

4. Objek perangkat yang memiliki sertifikat disinkronkan ke Azure AD melalui Azure AD Koneksi. Siklus sinkronisasi adalah setiap 30 menit secara default, tetapi bergantung pada konfigurasi Azure AD Koneksi. Untuk informasi selengkapnya, silakan lihat dokumen [ini](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. Pada tahap ini, Anda akan dapat melihat perangkat subjek dalam status "Tertunda" di bawah Blade perangkat Portal Azure.

6. Pada pengguna berikutnya masuk Windows 10, pendaftaran akan selesai. 

**Catatan**: Jika Anda menggunakan VPN dan proses masuk logo akan mengakhiri konektivitas domain, Anda dapat memicu pendaftaran secara manual:
 1. Masalah dsregcmd /gabung secara lokal pada perintah admin atau secara jarak jauh melalui PSExec ke PC Anda. Misalnya, PsExec -s \\ win10client01 cmd, dsregcmd /join

 2. Untuk detail selengkapnya tentang masalah Gabung Hibrid, lihat [Memecahkan masalah perangkat.](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)
