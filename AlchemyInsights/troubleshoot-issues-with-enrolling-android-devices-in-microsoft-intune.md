---
title: Memecahkan masalah dengan mendaftarkan perangkat Android di Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 6b26b2d77bceb063090986ff4e20bc4a56bb1242
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/30/2019
ms.locfileid: "29655886"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Memecahkan masalah dengan mendaftarkan perangkat Android di Microsoft Intune

Tinjau sumber daya berikut untuk menyelesaikan masalah Anda sekarang.
  
Beberapa masalah umum dan langkah-langkah resolusi:
  
 **Perangkat tidak dienkripsi kesalahan dalam Portal perusahaan:** Versi Android, khususnya diawali v7.0, memerlukan passcode startup untuk memastikan bahwa perangkat Anda dienkripsi penuh. Solusi umum akan mengaktifkan startup pin atau sepenuhnya mengenkripsi perangkat. Meninjau [dokumen ini](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) untuk informasi lebih lanjut. 
  
 **Perangkat gagal untuk check-in Layanan Intune atau menampilkan sebagai "Tidak sehat" di konsol admin Intune:** Beberapa 4.4 Samsung dan 5.5 perangkat tidak dapat memeriksa ke layanan. Ada 3 kemungkinan solusi untuk masalah ini: 
  
1. Secara manual membuka app Intune perusahaan Portal, yang akan secara otomatis memulai sinkronisasi perangkat.
    
2. Memperbarui perangkat untuk Android 6.0 atau lebih tinggi.
    
3. Menonaktifkan Samsung Smart Manager dari mengelola Intune Portal perusahaan. Meninjau [dokumen ini](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) untuk rincian lebih lanjut pada masalah ini dan resolusi. 
    
 **Pengguna lisensi jenis tidak valid** atau **kesalahan pengguna nama tidak dikenali:** kebutuhan pengguna akan diberikan izin Intune atau EMS. Meninjau dokumen-dokumen ini untuk menetapkan lisensi melalui: portal kantor Admin Center atau Azure. 
  
Sumber daya tambahan untuk membantu menyelesaikan masalah Anda:
  
1. Gunakan [Intune pemecahan masalah Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) untuk mendiagnosa dan mengatasi gangguan pendaftaran umum. Meninjau [dokumen ini](https://docs.microsoft.com/intune/help-desk-operators) untuk rincian lebih lanjut. 
    
2. Meninjau [dokumen ini](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) untuk daftar kesalahan umum yang mencegah pendaftaran dan resolusi untuk masing-masing. 
    
3. [Belajar bagaimana untuk mendaftar perangkat Android di Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
    

