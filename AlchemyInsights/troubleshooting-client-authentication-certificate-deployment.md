---
title: Pemecahan masalah penyebaran sertifikat autentikasi klien
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
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658989"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Pemecahan masalah penyebaran sertifikat autentikasi klien

Intune NDES/SCEP dan PKCS/PFX profil sertifikat klien biasanya digunakan bersama dengan tipe profil lain seperti WiFi, VPN, dan email untuk memperbolehkan pengguna mengautentikasi sumber daya perusahaan. Ketika tipe profil tersebut ditautkan ke profil sertifikat klien sangat tergantung pada keberhasilan penyebaran profil tersebut.

Penyetelan infrastruktur awal dan konfigurasi profil sertifikat klien sering kali memerlukan pemecahan masalah. Untuk panduan langkah demi langkah untuk penyiapan yang berhasil dari konektor NDES dan panduan pemecahan masalah untuk mengisolasi masalah dengan penyebaran sertifikat, lihat: 

- [Mengonfigurasi infrastruktur untuk mendukung SCEP dengan Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Gambaran umum untuk pemecahan masalah profil sertifikat SCEP dengan Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Gunakan skrip PowerShell yang direferensikan untuk membantu memverifikasi konfigurasi Anda. Untuk informasi selengkapnya, lihat [skrip verifikasi konektor sertifikat Intune](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Masalah umum lainnya**

**Ketika saya mencoba untuk menginstal konektor sertifikat Intune di server konektor NDES, saya mendapatkan pesan, "kata sandi dalam permintaan Sertifikat tidak dapat diverifikasi. Mungkin telah digunakan sudah. Dapatkan kata sandi baru untuk dikirim dengan permintaan ini. "**  

Pesan ini berarti Anda harus menjalankan instalasi konektor sertifikat sebagai administrator.

Di beberapa lingkungan, server tempat sertifikat Intune berjalan harus menggunakan server proksi untuk menyambungkan ke Intune, dan konektor sertifikat harus menggunakan proksi. Dalam beberapa situasi, konektor NDES mengabaikan pengaturan proksi yang dikonfigurasi, dan mungkin perlu mengonfigurasi pengaturan proksi saat berjalan dalam konteks keamanan LocalSystem. 
 
Solusinya adalah dengan menjalankan Internet Explorer sebagai sistem dan mengonfigurasi proksi di IE. Setelah memulai ulang layanan konektor Intune, konektor NDES tersambung ke Intune.

**Perangkat pengguna tidak lagi menerima sertifikat SCEP dari NDE.**

Dimungkinkan bahwa sertifikat autentikasi klien yang dikeluarkan untuk server NDE, dan ditentukan selama instalasi konektor NDES, telah kedaluwarsa atau hilang. Untuk mengatasi masalah: 
 
1. Hapus instalasi konektor NDES.  
2. Gunakan detail ini untuk meminta autentikasi klien baru atau sertifikat autentikasi server: 
 
    - Nama subjek: CN = eksternal FQDN  
    - Nama Alternatif subjek (keduanya diperlukan): DNS = FQDN eksternal, DNS = FQDN internal 
 
3. Instal ulang konektor NDES dengan sertifikat baru.