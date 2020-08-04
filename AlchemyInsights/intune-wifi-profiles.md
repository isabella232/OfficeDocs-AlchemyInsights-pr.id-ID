---
title: Profil Wi-Fi Intune
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
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555312"
---
# <a name="intune-wi-fi-profiles"></a>Profil Wi-Fi Intune

Keberhasilan implementasi konektivitas Wi-Fi untuk klien MDM tergantung pada profil yang disebarkan dengan benar yang mencerminkan persyaratan infrastruktur Wi-Fi perusahaan. Untuk meninjau pengaturan yang sesuai untuk platform klien yang sedang Anda selidiki, lihat: 

[Menambahkan pengaturan Wi-Fi untuk perangkat yang menjalankan Android di Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android)

[Menambahkan setelan Wi-Fi untuk perangkat Android Enterprise khusus dan terkelola sepenuhnya di Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[Menambahkan pengaturan Wi-Fi untuk perangkat iOS dan iPadOS di Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[Menambahkan pengaturan Wi-Fi untuk Windows 10 dan perangkat yang lebih baru di Intune](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[Mengimpor setelan Wi-Fi untuk perangkat Windows di Intune](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**Masalah umum**

**Saya menerapkan profil Wi-Fi yang bergantung pada sertifikat yang disebarkan yang ditentukan di profil Wi-Fi. Namun, profil konfigurasi menunjukkan status galat.**

Periksa apakah perangkat Anda menerima sertifikat.

1. Di Intune, buka **semua perangkat** dan pilih perangkat > **konfigurasi perangkat**.

2. Periksa bahwa semua profil yang diharapkan terdaftar dan dalam keadaan yang berhasil.

3. Untuk profil Android, jika Anda memiliki sertifikat perantara dalam rantai sertifikat, pastikan mereka disebarkan ke perangkat Android.

    Untuk memeriksa status sertifikat, pergi ke profil **konfigurasi perangkat**  >  **Profiles**  >  **Android menengah CA**  >  **properti**  >  **sertifikat terpercaya**.

Jika Anda terus melihat kesalahan, Tinjau prosedur dan bagian pemecahan masalah. Untuk informasi lebih lanjut, lihat [Ikhtisar untuk pemecahan masalah profil sertifikat SCEP dengan Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).

**Saya menerapkan profil Wi-Fi ke perangkat. Intune menunjukkan bahwa itu berhasil, tetapi perangkat tidak terhubung ke Wi-Fi.**

Status berhasil berarti bahwa Intune telah berhasil menyebarkan profil sebagai dikonfigurasi. Namun, konfigurasi ini mungkin tidak cocok dengan persyaratan jaringan dan/atau autentikasi Anda. Untuk rincian lebih lanjut tentang percobaan sambungan, periksa log di infrastruktur dan otentikasi Layanan (pada titik akses Wi-Fi controller dan NPS/radius server). Anda mungkin harus bekerja sama dengan tim infrastruktur jaringan, atau vendor Wi-Fi pihak ketiga, untuk mengumpulkan dan meninjau log.