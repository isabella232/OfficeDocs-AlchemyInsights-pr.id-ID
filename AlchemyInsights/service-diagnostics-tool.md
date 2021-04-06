---
title: Alat diagnostik layanan untuk Windows Virtual Desktop
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595868"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Alat diagnostik layanan untuk Windows Virtual Desktop

Windows Virtual Desktop (WVD) menawarkan alat diagnostik yang memungkinkan admin mengidentifikasi kesalahan melalui satu antarmuka. Alat ini mencatat info terkait diagnostik setiap kali WVD digunakan oleh seseorang yang ditetapkan peran WVD. Setiap log berisi informasi tentang peran WVD yang dilibatkan dalam aktivitas, pesan kesalahan yang muncul selama sesi, dan informasi tentang penyewa dan pengguna. Analitik Log Azure dapat dikonfigurasi untuk merekam log aktivitas yang dibuat oleh alat diagnostik dengan mengikuti langkah-langkah berikut:

1. Buat ruang kerja Analitik Log dengan [portal Azure](https://go.microsoft.com/fwlink/?linkid=2129500) atau [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).

1. [Sambungkan komputer Windows ke Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913). Dapatkan ID Ruang Kerja dan Kunci Utama ruang kerja Anda. Panduan penyiapan memerlukan informasi ini untuk mengonfigurasi agen dengan benar dan memastikannya dapat berkomunikasi dengan Azure Monitor.

1. [Mendorong data diagnostik ke ruang kerja Anda.](https://go.microsoft.com/fwlink/?linkid=2128284) Anda bisa mendorong data diagnostik dari penyewa WVD Anda ke Analitik Log untuk ruang kerja Anda.

1. [Identifikasi dan mendiagnosis](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) masalah yang bersesalifikasi internal maupun eksternal sehubungan dengan WVD.

Untuk mempelajari selengkapnya tentang mengonfigurasi alat diagnostik layanan untuk WVD, lihat Menggunakan Analitik Log untuk fitur diagnostik.