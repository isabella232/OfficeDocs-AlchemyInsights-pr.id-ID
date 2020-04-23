---
title: Memecahkan masalah dengan mendaftarkan perangkat iOS di Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 664c18daca5d8e0ad4a88f41db3ff0dbced606e5
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43736161"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Memecahkan masalah dengan mendaftarkan perangkat iOS di Microsoft Intune

Tinjau sumber daya yang tercantum di bawah ini untuk menyelesaikan masalah Anda sekarang. 
  
Beberapa pesan error dan langkah resolusi umum:
  
- **Cap perangkat tercapai** Pengguna memiliki lebih banyak perangkat yang terdaftar daripada batas perangkat. Tinjau dokumen ini untuk [menghapus perangkat](https://docs.microsoft.com/intune/devices-wipe) atau [mengubah batas perangkat](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Layanan ini tidak didukung. Tidak ada kebijakan pendaftaran:** Layanan pemberitahuan push Apple (APNS) perlu dikonfigurasi atau diperpanjang. Tinjau [dokumen ini](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) untuk mendapatkan petunjuk tentang cara melakukannya. 
    
- **Jenis lisensi pengguna tidak valid atau nama pengguna tidak dikenali:** Pengguna harus ditetapkan Intune atau EMS lisensi. Tinjau dokumen ini untuk menetapkan lisensi melalui: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) atau [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Sumber daya tambahan untuk membantu menyelesaikan masalah Anda:
  
1. Gunakan [Intune pemecahan masalah portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) untuk mendiagnosis dan menyelesaikan umum kegagalan pendaftaran. Tinjau [dokumen ini](https://docs.microsoft.com/intune/help-desk-operators) untuk detail selengkapnya. 
    
2. Tinjau dokumen ini untuk daftar kesalahan umum yang mencegah pendaftaran dan resolusi untuk masing-masing: [panduan pemecahan](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) masalah dan [pemecahan masalah dokumen](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Pelajari cara mendaftarkan perangkat iOS di Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

