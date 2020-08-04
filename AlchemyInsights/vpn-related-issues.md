---
title: Masalah terkait VPN
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
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555235"
---
# <a name="vpn-related-issues"></a>Masalah terkait VPN

Keberhasilan pelaksanaan konektivitas VPN untuk MDM klien tergantung pada profil disebarkan yang benar mencerminkan persyaratan infrastruktur VPN. Untuk pengaturan yang sesuai untuk platform klien yang sedang Anda selidiki, lihat: 

[Windows 10 dan Windows Holographic pengaturan perangkat untuk menambahkan sambungan VPN menggunakan Intune](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[Menambahkan pengaturan VPN pada perangkat iOS dan iPadOS di Microsoft Intune](https://docs.microsoft.com/intune/vpn-settings-ios)  
[Pengaturan perangkat Android untuk mengkonfigurasi VPN di Intune](https://docs.microsoft.com/intune/vpn-settings-android)  
[Menambahkan pengaturan VPN pada perangkat macOS di Microsoft Intune](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

Jika profil VPN Anda menggunakan otentikasi berbasis sertifikat, pastikan bahwa sertifikat akar dan klien otentikasi sertifikat profil tertaut ke profil VPN disebarkan berhasil.

**Masalah umum**

**Saya menerapkan profil VPN ke perangkat. Intune menunjukkan bahwa itu berhasil, tetapi perangkat tidak terhubung ke VPN.**

Status berhasil berarti bahwa Intune telah berhasil menyebarkan profil sebagai dikonfigurasi. Namun, konfigurasi ini mungkin tidak cocok dengan persyaratan jaringan dan/atau autentikasi Anda. Tinjau log dalam infrastruktur dan otentikasi Layanan (di VPN server dan NPS/radius server) untuk rincian lebih lanjut tentang percobaan sambungan. Anda mungkin harus bekerja sama dengan tim infrastruktur jaringan, atau vendor VPN pihak ketiga, untuk mengumpulkan dan meninjau log.

**Saat saya mengonfigurasi VPN khusus untuk iOS, fitur VPN per aplikasi tidak tersedia.**

VPN per aplikasi untuk perangkat iOS di Intune saat ini tersedia untuk daftar penyedia dan mitra tertentu, yang juga harus memenuhi prasyarat sertifikat sebelum mengonfigurasi VPN per aplikasi. Untuk informasi lebih lanjut, lihat [mengatur per aplikasi Virtual Private Network (VPN) untuk IOS/iPadOS perangkat di Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app). 

Untuk informasi lebih lanjut tentang semua jenis sambungan VPN di Intune, lihat [membuat profil vpn untuk menyambung ke server VPN di Intune](https://docs.microsoft.com/intune/vpn-settings-configure).  

**VPN on-demand iOS tidak memicu ketika domain yang dikonfigurasi diakses**

Untuk menguji pengaturan VPN otomatis, tetapkan nilai berikut:

Saya ingin melakukan hal berikut: **mengevaluasi setiap upaya koneksi** 

Memilih apakah akan menghubungkan: **Hubungkan jika diperlukan**

Ketika pengguna mengakses domain ini: **target** *nama domain*

Jika konfigurasi di atas tidak berhasil, tambahkan elemen berikut:

Ketika URL ini tidak terjangkau, memaksa menghubungkan VPN: **Badurl**