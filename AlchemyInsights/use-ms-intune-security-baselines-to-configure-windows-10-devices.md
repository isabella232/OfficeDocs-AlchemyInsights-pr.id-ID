---
title: Menggunakan baseline keamanan Microsoft Intune untuk mengonfigurasi perangkat Windows 10
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573539"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Menggunakan baseline keamanan Microsoft Intune untuk mengonfigurasi perangkat Windows 10

Dasar-dasar keamanan Intune membantu melindungi pengguna dan perangkat. Baseline keamanan adalah grup yang dikonfigurasi sebelumnya dari pengaturan Windows yang digunakan untuk menerapkan grup pengaturan dan nilai default yang diketahui yang direkomendasikan oleh tim keamanan yang relevan. Dengan membuat profil baseline keamanan di Intune, Anda membuat Templat yang terdiri dari beberapa profil konfigurasi perangkat.

Saat Anda menggunakan baseline keamanan untuk grup pengguna atau perangkat, pengaturan diterapkan ke perangkat yang berjalan di Windows 10 atau yang lebih baru. Misalnya, Baseline Security baseline secara otomatis (1) memungkinkan BitLocker untuk drive yang dapat dilepas, (2) memerlukan kata sandi untuk membuka kunci perangkat, dan (3) menonaktifkan autentikasi dasar. Jika nilai default tidak berfungsi untuk lingkungan Anda, kustomisasi baseline untuk menerapkan pengaturan yang Anda perlukan.

Baseline keamanan juga membantu membuat alur kerja aman menyeluruh di Microsoft 365. Berikut ini adalah beberapa manfaat dari hal ini:

- Baseline keamanan menyertakan praktik terbaik dan saran untuk pengaturan yang mempengaruhi keamanan. Karena mitra Intune dengan tim keamanan Windows yang membuat baseline untuk kebijakan grup, rekomendasi ini didasarkan pada panduan yang solid dan pengalaman yang luas.
- Jika Anda baru menggunakan Intune dan tidak yakin tempat memulainya, baseline keamanan akan membantu Anda membuat dan menggunakan profil aman dengan cepat.
- Jika saat ini Anda menggunakan kebijakan grup, maka migrasi ke Intune untuk tujuan manajemen jauh lebih mudah dengan baseline keamanan, karena dibangun ke dalam Intune dan menyertakan kapabilitas terdepan untuk manajemen.

Untuk mempelajari selengkapnya, lihat [baseline keamanan Windows](https://go.microsoft.com/fwlink/?linkid=2141503) dan [manajemen perangkat seluler](https://go.microsoft.com/fwlink/?linkid=2141701).