---
title: Menggunakan profil email dengan Intune
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
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555253"
---
# <a name="using-email-profiles-with-intune"></a>Menggunakan profil email dengan Intune

Intune dapat digunakan untuk membuat dan menyebarkan profil email untuk klien email Native (built-in) pada beberapa platform perangkat.

Untuk informasi tentang beberapa pembatasan yang terkait dengan profil email, termasuk bagaimana keberadaan profil yang ada ditangani dan cara menghapus profil email, lihat [menambahkan pengaturan email ke perangkat menggunakan Intune](https://docs.microsoft.com/intune/email-settings-configure).

Untuk informasi lebih lanjut tentang cara membuat profil email untuk setiap platform perangkat, lihat:

[Pengaturan perangkat Android untuk mengkonfigurasi email, otentikasi, dan sinkronisasi di Intune](https://docs.microsoft.com/intune/email-settings-android)  
[Menambahkan pengaturan e-mail untuk perangkat iOS dan iPadOS di Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Tataan profil email di Microsoft Intune untuk perangkat yang menjalankan Windows Phone 8,1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Pengaturan profil email untuk perangkat yang menjalankan Windows 10 di Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Masalah sinkronisasi Umum**

**Sebuah KNOX pada profil email Android mencegah pengguna kontak, kalender, dan tugas, dari yang akan disinkronkan ke perangkat pengguna.**

The KNOX di profil email Android KNOX menawarkan admin pilihan untuk memutuskan jenis konten yang akan disinkronkan ke perangkat dengan menetapkan masing-masing untuk diaktifkan.

Jika setelan untuk jenis konten apa pun diatur ke **tidak dikonfigurasi** (default), jenis konten tersebut tidak disinkronkan secara otomatis. Pengguna dapat mengaktifkan jenis konten yang mereka inginkan secara langsung pada perangkat secara manual, tetapi konfigurasi yang akan ditimpa oleh Intune pengaturan kebijakan, dan sinkronisasi berhenti untuk jenis konten tersebut.

