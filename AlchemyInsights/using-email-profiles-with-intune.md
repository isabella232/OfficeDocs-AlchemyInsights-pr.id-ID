---
title: Menggunakan profil email dengan Intune
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
- "1559"
- "9000076"
ms.openlocfilehash: b1653b73e7296e7eed411ae73c19342a1187b2eb7e287cff4339ea0ca32d75c1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53919426"
---
# <a name="using-email-profiles-with-intune"></a>Menggunakan profil email dengan Intune

Intune dapat digunakan untuk membuat dan menyebarkan profil email untuk klien email asli (bawaan) pada beberapa platform perangkat.

Untuk informasi tentang beberapa batasan yang terkait dengan profil email, termasuk bagaimana kehadiran profil yang sudah ada ditangani dan cara menghapus profil email, lihat Menambahkan pengaturan email ke perangkat menggunakan [Intune](https://docs.microsoft.com/intune/email-settings-configure).

Untuk informasi selengkapnya tentang cara membuat profil email untuk setiap platform perangkat, lihat:

[Pengaturan perangkat Android untuk mengonfigurasi email, autentikasi, dan sinkronisasi di Intune](https://docs.microsoft.com/intune/email-settings-android)  
[Menambahkan pengaturan email untuk perangkat iOS dan iPadOS di Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Pengaturan profil email di Microsoft Intune untuk perangkat yang menjalankan Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Pengaturan profil email untuk perangkat yang Windows 10 di Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Masalah sinkronisasi umum**

**Knox pada profil email Android mencegah kontak, Kalender, dan Tugas pengguna, tidak disinkronkan ke perangkat pengguna.**

Profil email KNOX di Android KNOX menawarkan opsi kepada admin untuk memutuskan tipe konten mana yang disinkronkan ke perangkat dengan mengatur masing-masing tipe konten agar diaktifkan.

Jika pengaturan untuk salah satu tipe  konten diatur ke Tidak dikonfigurasi (default), tipe konten tersebut tidak disinkronkan secara otomatis. Pengguna mungkin mengaktifkan tipe konten yang mereka inginkan secara langsung di perangkat secara manual, tetapi konfigurasi itu ditimpa oleh pengaturan kebijakan Intune, dan sinkronisasi berhenti untuk tipe konten itu.

