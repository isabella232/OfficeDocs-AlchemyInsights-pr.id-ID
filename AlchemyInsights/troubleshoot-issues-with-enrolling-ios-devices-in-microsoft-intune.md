---
title: Memecahkan masalah dengan mendaftarkan perangkat iOS di Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 663ff9b101494be781095ca550a4ed3deedca175
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/15/2019
ms.locfileid: "28295595"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Memecahkan masalah dengan mendaftarkan perangkat iOS di Microsoft Intune

Tinjau sumber daya berikut untuk menyelesaikan masalah Anda sekarang. 
  
Beberapa pesan kesalahan umum dan langkah-langkah resolusi:
  
- **Perangkat Cap mencapai** Pengguna memiliki lebih perangkat yang terdaftar dari batas perangkat. Meninjau dokumen-dokumen ini untuk [menghapus perangkat](https://docs.microsoft.com/en-us/intune/devices-wipe) atau [mengubah batas perangkat](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Layanan ini tidak didukung. Tidak ada kebijakan pendaftaran:** Apple mendorong pemberitahuan Layanan (APNS) perlu dikonfigurasi atau diperbaharui. Meninjau [dokumen ini](https://docs.microsoft.com/en-us/intune/apple-mdm-push-certificate-get) untuk petunjuk tentang cara untuk melakukan itu. 
    
- **Pengguna lisensi jenis valid atau nama pengguna tidak dikenal:** Kebutuhan pengguna akan diberikan izin Intune atau EMS. Meninjau dokumen-dokumen ini untuk menetapkan lisensi melalui: [Kantor Admin Center](https://docs.microsoft.com/en-us/intune/licenses-assign) atau [Azure portal](https://docs.microsoft.com/en-us/azure/active-directory/license-users-groups).
    
Sumber daya tambahan untuk membantu menyelesaikan masalah Anda:
  
1. Gunakan [Intune pemecahan masalah Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) untuk mendiagnosa dan mengatasi gangguan pendaftaran umum. Meninjau [dokumen ini](https://docs.microsoft.com/en-us/intune/help-desk-operators) untuk rincian lebih lanjut. 
    
2. Meninjau dokumen-dokumen ini untuk daftar kesalahan umum yang mencegah pendaftaran dan resolusi untuk masing-masing: [panduan mengatasi masalah](https://support.microsoft.com/en-us/help/4039809/troubleshooting-ios-device-enrollment-in-intune) dan [mengatasi masalah doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Belajar bagaimana untuk mendaftar perangkat iOS di Microsoft Intune](https://docs.microsoft.com/en-us/intune/ios-enroll).
    

