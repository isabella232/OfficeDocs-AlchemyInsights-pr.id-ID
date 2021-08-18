---
title: Masalah penginstalan Pertahanan Microsoft di Mac atau Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: defc11265caf371ce0a62a10a5de1d8ff88a8e11
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325252"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Masalah penginstalan Pertahanan Microsoft di Mac atau Linux

**Mac**

- Pastikan bahwa persyaratan sistem telah terpenuhi sebelum menginstal ATP Pertahanan Microsoft untuk Mac. Untuk informasi selengkapnya, [lihat Cara menginstal ATP Pertahanan Microsoft untuk Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).  
- Tinjau informasi dalam file: "/Library/Logs/Microsoft/mdatp/install.log".

**Linux**

- Pastikan bahwa persyaratan sistem telah terpenuhi sebelum menginstal ATP Pertahanan Microsoft untuk Linux. Untuk informasi selengkapnya, [lihat Cara menginstal MDATP untuk Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements). 
- Untuk memverifikasi bahwa layanan MDATP sedang berjalan, [lihat Penginstalan gagal.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)  
    Untuk memecahkan dan mengatasi masalah jika layanan tidak berjalan, lihat [Langkah-langkah untuk memecahkan masalah jika layanan mdatp tidak berjalan.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)
- Untuk langkah-langkah untuk memeriksa konfigurasi klien, yang memverifikasi kesehatan produk, dan untuk menjalankan uji deteksi pada file teks EICAR, lihat [Konfigurasi klien](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).  

    **Catatan** Untuk daftar sistem file yang didukung untuk aktivitas akses, lihat [ATP Pertahanan Microsoft untuk Linux.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)