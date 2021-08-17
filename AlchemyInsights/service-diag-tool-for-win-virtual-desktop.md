---
title: Alat diagnostik layanan untuk Windows Desktop Virtual
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: 58688e3216ba6777b1a4f76095bd39c81a2d2a8294e06b6bc61c7134f6d589f9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052389"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Alat diagnostik layanan untuk Windows Desktop Virtual

Windows Desktop Virtual (WVD) menawarkan alat diagnostik yang memungkinkan admin mengidentifikasi kesalahan melalui satu antarmuka. Alat ini mencatat info terkait diagnostik setiap kali WVD digunakan oleh seseorang yang ditetapkan peran WVD. Setiap log berisi informasi tentang peran WVD yang dilibatkan dalam aktivitas, pesan kesalahan yang muncul selama sesi, dan informasi tentang penyewa dan pengguna. Analitik Log Azure dapat dikonfigurasi untuk merekam log aktivitas yang dibuat oleh alat diagnostik. Berikut caranya:

1. Buat ruang kerja Analitik Log dengan [portal Azure atau Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129500) . [](https://go.microsoft.com/fwlink/?linkid=2129501)
1. [Koneksi Windows baru ke Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913). Dapatkan ID Ruang Kerja dan Kunci Utama ruang kerja Anda. Panduan penyiapan memerlukan informasi ini untuk mengonfigurasi agen dengan benar dan memastikannya dapat berkomunikasi dengan Azure Monitor.
1. [Mendorong data diagnostik ke ruang kerja Anda.](https://go.microsoft.com/fwlink/?linkid=2128284) Anda bisa mendorong data diagnostik dari penyewa WVD Anda ke Analitik Log untuk ruang kerja Anda.
1. [Identifikasi dan mendiagnosis](https://go.microsoft.com/fwlink/?linkid=2128338) masalah yang bersesalifikasi internal maupun eksternal sehubungan dengan WVD.

Untuk mempelajari selengkapnya tentang mengonfigurasi alat diagnostik layanan untuk WVD, lihat [Menggunakan Analitik Log untuk fitur diagnostik](https://go.microsoft.com/fwlink/?linkid=2128084).
