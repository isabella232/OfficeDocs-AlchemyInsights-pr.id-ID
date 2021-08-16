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
ms.openlocfilehash: 6646ca4792ac4d9fb8bfb7433d53ecf4aeba8da0aca797225c16c02b28499889
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013247"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Masalah penginstalan Pertahanan Microsoft di Mac atau Linux

**Mac**

- Pastikan bahwa persyaratan sistem telah terpenuhi sebelum menginstal ATP Pertahanan Microsoft untuk Mac. Untuk informasi selengkapnya, [lihat Cara menginstal ATP Pertahanan Microsoft untuk Mac](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).  
- Tinjau informasi dalam file: "/Library/Logs/Microsoft/mdatp/install.log".

**Linux**

- Pastikan bahwa persyaratan sistem telah terpenuhi sebelum menginstal ATP Pertahanan Microsoft untuk Linux. Untuk informasi selengkapnya, [lihat Cara menginstal MDATP untuk Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements). 
- Untuk memverifikasi bahwa layanan MDATP sedang berjalan, [lihat Penginstalan gagal.](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)  
    Untuk memecahkan dan mengatasi masalah jika layanan tidak berjalan, lihat [Langkah-langkah untuk memecahkan masalah jika layanan mdatp tidak berjalan.](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)
- Untuk langkah-langkah untuk memeriksa konfigurasi klien, yang memverifikasi kesehatan produk, dan untuk menjalankan uji deteksi pada file teks EICAR, lihat [Konfigurasi klien](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).  

    **Catatan** Untuk daftar sistem file yang didukung untuk aktivitas akses, lihat [ATP Pertahanan Microsoft untuk Linux.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)