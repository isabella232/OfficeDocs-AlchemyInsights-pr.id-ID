---
title: Alat diagnostik layanan untuk Desktop Virtual Windows
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
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/14/2020
ms.locfileid: "49678623"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Alat diagnostik layanan untuk Desktop Virtual Windows

Windows Virtual desktop (WVD) menawarkan alat diagnostik yang memungkinkan admin mengidentifikasi kesalahan melalui satu antarmuka. Alat ini mencatat informasi terkait diagnostik setiap kali WVD digunakan oleh seseorang yang ditugaskan sebagai peran WVD. Setiap log berisi info tentang peran WVD yang terlibat dalam aktivitas, pesan kesalahan yang muncul selama sesi, dan informasi tentang penyewa dan pengguna. Analitik log Azure bisa dikonfigurasikan untuk merekam log aktivitas yang dibuat oleh alat diagnostik. Berikut caranya:

1. Membuat ruang kerja analitik log dengan [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) atau [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).
1. [Sambungkan komputer Windows ke Azure monitor](https://go.microsoft.com/fwlink/?linkid=2129913). Dapatkan ID ruang kerja dan kunci utama ruang kerja Anda. Panduan penyetelan memerlukan info ini untuk mengonfigurasi agen dengan benar dan memastikan bahwa alat tersebut dapat berkomunikasi dengan Azure monitor.
1. [Dorong diagnostik data ke ruang kerja Anda](https://go.microsoft.com/fwlink/?linkid=2128284). Anda dapat mendorong diagnostik data dari penyewa WVD ke log analitik untuk ruang kerja Anda.
1. [Mengidentifikasi dan mendiagnosis masalah](https://go.microsoft.com/fwlink/?linkid=2128338) yang bersifat internal atau eksternal dalam kaitannya dengan wvd.

Untuk mempelajari selengkapnya tentang mengonfigurasi alat diagnostik layanan untuk WVD, lihat [menggunakan log analitik untuk fitur diagnostik](https://go.microsoft.com/fwlink/?linkid=2128084).
