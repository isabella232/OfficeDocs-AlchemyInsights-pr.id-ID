---
title: Pemecahan masalah penyebaran sertifikat otentikasi klien
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555307"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Pemecahan masalah penyebaran sertifikat otentikasi klien

Intune NDES/SCEP dan PKCS/PFX klien sertifikat profil yang umum digunakan bersama dengan jenis profil lain seperti WiFi, VPN, dan email untuk memungkinkan pengguna untuk mengotentikasi ke sumber daya perusahaan. Ketika jenis profil tersebut tertaut ke profil sertifikat klien tergantung pada penyebaran berhasil profil tersebut.

Penataan infrastruktur awal dan konfigurasi terkait profil sertifikat klien sering memerlukan pemecahan masalah. Untuk panduan selangkah demi selangkah untuk berhasil penataan konektor NDES dan panduan pemecahan masalah untuk mengisolasi masalah dengan penyebaran sertifikat, lihat: 

- [Mengkonfigurasi infrastruktur untuk mendukung SCEP dengan Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Ikhtisar untuk pemecahan masalah profil sertifikat SCEP dengan Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Gunakan skrip PowerShell yang direferensikan untuk membantu memverifikasi konfigurasi Anda. Untuk informasi lebih lanjut, lihat [Intune sertifikat konektor verifikasi skrip](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Masalah umum lainnya**

**Ketika saya mencoba untuk menginstal konektor sertifikat Intune di server konektor NDES, saya mendapatkan pesan, "sandi di sertifikat permintaan tidak dapat diverifikasi. Ini mungkin telah digunakan sudah. Dapatkan kata sandi baru untuk dikirimkan dengan permintaan ini. "**  

Pesan ini berarti bahwa Anda harus menjalankan penginstalan konektor sertifikat sebagai administrator.

Di beberapa lingkungan, server di mana Intune sertifikat berjalan harus menggunakan server proksi untuk menyambung ke Intune, dan konektor sertifikat harus menggunakan proksi. Dalam beberapa keadaan, konektor NDES mengabaikan pengaturan proksi dikonfigurasi, dan mungkin perlu untuk mengkonfigurasi pengaturan proxy saat berjalan dalam konteks keamanan LocalSystem. 
 
Solusinya adalah dengan menjalankan Internet Explorer sebagai sistem dan mengkonfigurasi proxy di IE. Setelah restart layanan konektor Intune, konektor NDES menyambung ke Intune.

**Perangkat pengguna tidak lagi menerima SCEP sertifikat dari NDES.**

Dimungkinkan bahwa sertifikat otentikasi klien yang dikeluarkan untuk NDES server, dan ditentukan selama penginstalan konektor NDES, telah kedaluwarsa atau hilang. Untuk menyelesaikan: 
 
1. Membongkar konektor NDES.  
2. Gunakan rincian ini untuk meminta otentikasi klien baru atau sertifikat otentikasi server: 
 
    - Nama subjek: CN = FQDN eksternal  
    - Nama Alternatif subjek (keduanya diperlukan): DNS = eksternal FQDN, DNS = internal FQDN 
 
3. Instal ulang konektor NDES dengan sertifikat baru.