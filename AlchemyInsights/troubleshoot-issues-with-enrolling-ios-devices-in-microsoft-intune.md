---
title: Memecahkan masalah dengan mendaftarkan perangkat iOS di Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: d28dca4fccf823e627dd179f828ba3b8baf843a6
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/23/2019
ms.locfileid: "32391010"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Memecahkan masalah dengan mendaftarkan perangkat iOS di Microsoft Intune

Tinjau sumber daya berikut untuk menyelesaikan masalah Anda sekarang. 
  
Beberapa pesan kesalahan umum dan langkah-langkah resolusi:
  
- **Perangkat Cap mencapai** Pengguna memiliki lebih perangkat yang terdaftar dari batas perangkat. Meninjau dokumen-dokumen ini untuk [menghapus perangkat](https://docs.microsoft.com/intune/devices-wipe) atau [mengubah batas perangkat](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Layanan ini tidak didukung. Tidak ada kebijakan pendaftaran:** Apple mendorong pemberitahuan Layanan (APNS) perlu dikonfigurasi atau diperbaharui. Meninjau [dokumen ini](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) untuk petunjuk tentang cara untuk melakukan itu. 
    
- **Pengguna lisensi jenis valid atau nama pengguna tidak dikenal:** Kebutuhan pengguna akan diberikan izin Intune atau EMS. Meninjau dokumen-dokumen ini untuk menetapkan lisensi melalui: [Kantor Admin Center](https://docs.microsoft.com/intune/licenses-assign) atau [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Sumber daya tambahan untuk membantu menyelesaikan masalah Anda:
  
1. Gunakan [Intune pemecahan masalah Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) untuk mendiagnosa dan mengatasi gangguan pendaftaran umum. Meninjau [dokumen ini](https://docs.microsoft.com/intune/help-desk-operators) untuk rincian lebih lanjut. 
    
2. Meninjau dokumen-dokumen ini untuk daftar kesalahan umum yang mencegah pendaftaran dan resolusi untuk masing-masing: [panduan mengatasi masalah](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) dan [mengatasi masalah doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Belajar bagaimana untuk mendaftar perangkat iOS di Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

