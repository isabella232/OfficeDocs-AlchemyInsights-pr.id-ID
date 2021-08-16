---
title: Pemecahan masalah penyebaran sertifikat Autentikasi Klien
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 78520b416a72a3c93a3d2e7726948d59f83e681d4f09078c2a3cefac7bf1db3d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020807"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Pemecahan masalah penyebaran sertifikat Autentikasi Klien

Profil sertifikat Klien Intune NDES/SCEP dan PKCS/PFX Client umumnya digunakan bersama dengan tipe profil lainnya seperti Wifi, VPN, dan email untuk memungkinkan pengguna mengautentikasi ke sumber daya perusahaan. Ketika tipe profil tersebut ditautkan ke profil sertifikat klien bergantung pada berhasilnya penyebaran profil tersebut.

Penyetelan infrastruktur awal dan konfigurasi terkait profil Sertifikat Klien sering memerlukan pemecahan masalah. Untuk panduan langkah demi langkah agar penyiapan konektor NDES berhasil dan panduan pemecahan masalah untuk mengisolasi masalah dengan penyebaran sertifikat, lihat: 

- [Mengonfigurasi infrastruktur untuk mendukung SCEP dengan Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Gambaran umum untuk memecahkan masalah profil sertifikat SCEP dengan Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Menggunakan skrip powershell yang direferensikan untuk membantu memverifikasi konfigurasi Anda. Untuk informasi selengkapnya, lihat [Skrip verifikasi konektor Sertifikat Intune](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Masalah umum lainnya**

**Ketika mencoba menginstal konektor sertifikat Intune di server konektor NDES, saya mendapatkan pesan, "Kata sandi di permintaan sertifikat tidak dapat diverifikasi. Ini mungkin telah digunakan. Dapatkan kata sandi baru untuk dikirim dengan permintaan ini."**  

Pesan ini berarti Anda harus menjalankan instalasi konektor sertifikat sebagai Administrator.

Di beberapa lingkungan, server yang menjalankan Sertifikat Intune harus menggunakan server proksi untuk menyambungkan ke Intune, sehingga Konektor Sertifikat harus menggunakan proksi. Dalam beberapa situasi, NDES Connector mengabaikan pengaturan proksi yang dikonfigurasi, dan mungkin perlu mengonfigurasi pengaturan proksi saat berjalan dalam konteks keamanan LocalSystem. 
 
Solusinya adalah dengan menjalankan Internet Explorer sebagai SYSTEM dan mengonfigurasi proksi di IE. Setelah memulai ulang Intune Connector Service, Konektor NDES tersambung ke Intune.

**Perangkat pengguna tidak lagi menerima sertifikat SCEP dari NDES.**

Ada kemungkinan bahwa sertifikat Autentikasi Klien yang dikeluarkan untuk server NDES, dan yang ditentukan selama instalasi konektor NDES, telah kedaluwarsa atau hilang. Untuk mengatasinya: 
 
1. Hapus instalan konektor NDES.  
2. Gunakan detail ini untuk meminta sertifikat autentikasi klien atau server yang baru: 
 
    - Nama subjek: CN=fqdn eksternal  
    - Nama alternatif subjek (keduanya diperlukan): DNS=fqdn eksternal, DNS=fqdn internal 
 
3. Instal ulang konektor NDES dengan sertifikat yang baru.