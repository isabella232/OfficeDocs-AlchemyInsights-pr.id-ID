---
title: Memecahkan masalah dengan mendaftarkan perangkat iOS di Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708965"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Memecahkan masalah dengan mendaftarkan perangkat iOS di Microsoft Intune

Tinjau sumber daya yang tercantum di bawah ini untuk mengatasi masalah Anda sekarang. 
  
Beberapa langkah pemecahan masalah dan pesan kesalahan umum:
  
- **Kapitalisasi perangkat tercapai** Pengguna memiliki lebih banyak perangkat yang terdaftar dibandingkan batas perangkat. Tinjau dokumen ini untuk [menghapus perangkat](https://docs.microsoft.com/intune/devices-wipe) atau [mengubah batas perangkat](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Layanan ini tidak didukung. Tidak ada kebijakan pendaftaran:** Layanan pemberitahuan push Apple (APN) perlu dikonfigurasikan atau diperbarui. Tinjau [dokumen ini](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) untuk mendapatkan instruksi tentang cara melakukannya. 
    
- **Lisensi pengguna tipe tidak valid atau nama pengguna tidak dikenali:** Pengguna harus diberi lisensi Intune atau EMS. Tinjau dokumen ini untuk menetapkan lisensi melalui: [Pusat admin Office](https://docs.microsoft.com/intune/licenses-assign) atau [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Sumber daya tambahan untuk membantu mengatasi masalah Anda:
  
1. Gunakan [portal pemecahan masalah Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) untuk mendiagnosis dan mengatasi kegagalan pendaftaran umum. Tinjau [dokumen ini](https://docs.microsoft.com/intune/help-desk-operators) untuk detail selengkapnya. 
    
2. Tinjau dokumen ini untuk daftar kesalahan umum yang mencegah pendaftaran dan resolusi untuk masing-masing: [panduan pemecahan](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) masalah dan dokumen [pemecahan masalah](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).
    
3. [Pelajari cara mendaftarkan perangkat iOS di Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

