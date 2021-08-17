---
title: Menggunakan Microsoft Intune baseline keamanan untuk mengonfigurasi Windows 10 Anda
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
ms.openlocfilehash: a94c6b72df3874ee80413adac86d60306175734b6ff28b2e015e05eec6f3838b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104347"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Menggunakan Microsoft Intune baseline keamanan untuk mengonfigurasi Windows 10 Anda

Baseline keamanan Intune membantu melindungi pengguna dan perangkat. Baseline keamanan adalah Windows yang telah dikonfigurasi sebelumnya dari pengaturan, yang digunakan untuk menerapkan grup pengaturan umum dan nilai default yang direkomendasikan oleh tim keamanan yang relevan. Dengan membuat profil baseline keamanan di Intune, Anda membuat templat yang terdiri dari beberapa profil konfigurasi perangkat.

Saat Anda menerapkan baseline keamanan ke sejumlah pengguna atau perangkat, pengaturan akan diterapkan ke perangkat yang dijalankan di Windows 10 baru. Misalnya, MDM Security Baseline secara otomatis (1) mengaktifkan BitLocker untuk drive yang dapat dilepas, (2) memerlukan kata sandi untuk membuka kunci perangkat, dan (3) menonaktifkan autentikasi dasar. Ketika nilai default tidak berfungsi untuk lingkungan Anda, kustomisasikan garis dasar untuk menerapkan pengaturan yang Anda perlukan.

Baseline keamanan juga membantu menetapkan alur kerja aman secara end-to-end Microsoft 365. Berikut adalah beberapa manfaat dari hal ini:

- Baseline keamanan mencakup praktik terbaik dan rekomendasi untuk pengaturan yang mempengaruhi keamanan. Karena Intune bermitra dengan Windows keamanan grup yang membuat baseline untuk kebijakan grup, rekomendasi ini didasarkan pada panduan yang solid dan pengalaman ekstensif.
- Jika Anda baru menggunakan Intune dan tidak yakin dari mana memulai, baseline keamanan akan membantu Anda membuat dan menggunakan profil yang aman dengan cepat.
- Jika saat ini Anda menggunakan kebijakan grup, migrasi ke Intune untuk tujuan manajemen jauh lebih mudah dengan baseline keamanan, karena baseline keamanan disertakan dalam Intune dan menyertakan kapabilitas yang canggih untuk manajemen.

Untuk mempelajari selengkapnya, lihat [Windows dasar keamanan dan](https://go.microsoft.com/fwlink/?linkid=2141503) Manajemen perangkat [seluler](https://go.microsoft.com/fwlink/?linkid=2141701).