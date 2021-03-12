---
title: Masalah penginstalan Microsoft Defender di Mac atau Linux
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
ms.openlocfilehash: a8d5ad2246b9b83e1e0a4d5be4dd8bb41c16e734
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "50713837"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Masalah penginstalan Microsoft Defender di Mac atau Linux

**Mak**

- Pastikan persyaratan sistem terpenuhi sebelum menginstal Microsoft Defender ATP untuk Mac. Untuk informasi selengkapnya, lihat [cara menginstal Microsoft Defender ATP untuk Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).  
- Tinjau informasi dalam file: "/Library/Logs/Microsoft/mdatp/install.log".

**Linux**

- Pastikan persyaratan sistem terpenuhi sebelum menginstal Microsoft Defender ATP untuk Linux. Untuk informasi selengkapnya, lihat [cara menginstal Microsoft Defender ATP untuk Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements). 
- Untuk memverifikasi bahwa layanan MDATP berjalan, lihat [penginstalan gagal](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).  
    Untuk memecahkan masalah dan mengatasi masalah jika Layanan tidak berjalan, lihat [langkah-langkah untuk memecahkan masalah jika Layanan mdatp tidak berjalan](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).
- Untuk langkah-langkah untuk memeriksa konfigurasi klien, yang memverifikasi kesehatan produk, dan menjalankan uji deteksi pada file teks EICAR, lihat [konfigurasi klien](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).  

    **Catatan** Untuk daftar sistem file yang didukung untuk aktivitas di tempat, lihat [Microsoft Defender ATP untuk Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).