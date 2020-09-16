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
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653291"
---
# <a name="using-email-profiles-with-intune"></a>Menggunakan profil email dengan Intune

Intune dapat digunakan untuk membuat dan menggunakan profil email untuk klien email bawaan (bawaan) di beberapa platform perangkat.

Untuk informasi tentang beberapa larangan yang terkait dengan profil email, termasuk bagaimana kehadiran profil yang sudah ditangani dan cara menghapus profil email, lihat [menambahkan pengaturan email ke perangkat yang menggunakan Intune](https://docs.microsoft.com/intune/email-settings-configure).

Untuk informasi selengkapnya tentang cara membuat profil email untuk setiap platform perangkat, lihat:

[Pengaturan perangkat Android untuk mengonfigurasi email, autentikasi, dan sinkronisasi di Intune](https://docs.microsoft.com/intune/email-settings-android)  
[Menambahkan pengaturan email untuk perangkat iOS dan iPadOS di Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Pengaturan profil email di Microsoft Intune untuk perangkat yang menjalankan Windows Phone 8,1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Pengaturan profil email untuk perangkat yang menjalankan Windows 10 di Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Masalah sinkronisasi Umum**

**KNOX pada profil email Android mencegah kontak, kalender, dan tugas pengguna, agar tidak disinkronkan dengan perangkat pengguna.**

Profil email KNOX di Android KNOX menawarkan admin opsi untuk memutuskan tipe konten mana yang disinkronkan ke perangkat dengan mengatur masing-masing untuk diaktifkan.

Jika pengaturan untuk salah satu tipe konten diatur ke **tidak dikonfigurasi** (default), tipe konten tersebut tidak disinkronkan secara otomatis. Pengguna mungkin mengaktifkan tipe konten yang mereka inginkan secara langsung di perangkat secara manual, tapi konfigurasi tersebut ditimpa dengan pengaturan kebijakan Intune, dan sinkronisasi berhenti untuk tipe konten tersebut.

