---
title: Menggunakan baseline keamanan Microsoft Intune untuk mengonfigurasi perangkat Windows 10
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/10/2021
ms.locfileid: "50694434"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a>Menggunakan baseline keamanan Microsoft Intune untuk mengonfigurasi perangkat Windows 10

Dasar-dasar keamanan Intune membantu melindungi pengguna dan perangkat. Baseline keamanan adalah grup yang dikonfigurasi sebelumnya dari pengaturan Windows yang digunakan untuk menerapkan grup pengaturan dan nilai default yang diketahui yang direkomendasikan oleh tim keamanan yang relevan. Dengan membuat profil baseline keamanan di Intune, Anda membuat Templat yang terdiri dari beberapa profil konfigurasi perangkat.

Saat Anda menggunakan baseline keamanan untuk grup pengguna atau perangkat, pengaturan diterapkan ke perangkat yang berjalan pada versi Windows 10 atau yang lebih baru. Misalnya, baseline keamanan manajemen perangkat seluler (MDM) Microsoft secara otomatis (1) memungkinkan BitLocker untuk drive yang dapat dilepas, (2) memerlukan kata sandi untuk membuka kunci perangkat, dan (3) menonaktifkan autentikasi dasar. Saat nilai default tidak berfungsi untuk lingkungan Anda, Anda bisa mengustomisasi baseline untuk menerapkan pengaturan yang Anda perlukan.

Baseline keamanan juga membantu membuat alur kerja aman menyeluruh di Microsoft 365. Berikut ini adalah beberapa manfaat dari fungsionalitas ini:
- Baseline keamanan menyertakan praktik terbaik dan saran untuk pengaturan yang mempengaruhi keamanan. Karena mitra Intune dengan tim keamanan Windows yang membuat baseline untuk kebijakan grup, rekomendasi ini didasarkan pada panduan yang solid dan pengalaman yang luas.
- Jika Anda baru menggunakan Intune dan tidak yakin tempat memulainya, baseline keamanan akan membantu Anda membuat dan menggunakan profil aman dengan cepat.
- Jika saat ini Anda menggunakan kebijakan grup, maka migrasi ke Intune untuk tujuan manajemen jauh lebih mudah dengan baseline keamanan, karena baseline keamanan ini dibangun ke dalam Intune dan menyertakan kapabilitas mutakhir untuk manajemen.

Untuk informasi selengkapnya, lihat baseline [keamanan Windows](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) dan [manajemen perangkat seluler](https://docs.microsoft.com/windows/client-management/mdm/).