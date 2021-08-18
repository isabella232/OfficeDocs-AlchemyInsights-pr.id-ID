---
title: Menggunakan Microsoft Intune baseline keamanan untuk mengonfigurasi Windows 10 Anda
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 911c6b1860e4f44e6d88897f73173cdd11060562
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331988"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Menggunakan Microsoft Intune baseline keamanan untuk mengonfigurasi Windows 10 Anda

Baseline keamanan Intune membantu melindungi pengguna dan perangkat. Baseline keamanan adalah Windows yang telah dikonfigurasi sebelumnya oleh grup yang digunakan untuk menerapkan grup pengaturan umum dan nilai default yang direkomendasikan oleh tim keamanan yang relevan. Dengan membuat profil baseline keamanan di Intune, Anda membuat templat yang terdiri dari beberapa profil konfigurasi perangkat.

Saat Anda menerapkan baseline keamanan ke sejumlah pengguna atau perangkat, pengaturan akan diterapkan ke perangkat yang dijalankan di Windows 10 baru. Misalnya, dasar keamanan manajemen perangkat seluler Microsoft (MDM) secara otomatis mengaktifkan BitLocker untuk drive yang dapat dilepas, memerlukan kata sandi untuk membuka kunci perangkat, dan menonaktifkan autentikasi dasar. Ketika nilai default tidak berfungsi untuk lingkungan Anda, Anda bisa mengkustomisasi garis dasar untuk menerapkan pengaturan yang Anda perlukan.

Baseline keamanan juga membantu menetapkan alur kerja aman secara end-to-end Microsoft 365. Baseline keamanan mencakup praktik terbaik dan rekomendasi untuk pengaturan yang mempengaruhi keamanan. Intune bermitra dengan Windows keamanan grup yang membuat baseline untuk kebijakan grup, sehingga rekomendasi ini didasarkan pada panduan yang solid dan pengalaman ekstensif.

Jika Anda baru menggunakan Intune dan tidak yakin dari mana memulai, baseline keamanan membantu Anda membuat dan menggunakan profil yang aman dengan cepat. Jika saat ini Anda menggunakan kebijakan grup, melakukan migrasi ke Intune untuk tujuan manajemen jauh lebih mudah dengan baseline keamanan karena baseline keamanan disertakan dalam Intune dan menyertakan kapabilitas manajemen yang canggih.

Untuk mempelajari selengkapnya, lihat [Windows dasar keamanan](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) dan Manajemen perangkat [seluler](https://docs.microsoft.com/windows/client-management/mdm/).

