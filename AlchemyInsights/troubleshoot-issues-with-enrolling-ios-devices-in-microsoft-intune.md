---
title: Memecahkan masalah pendaftaran perangkat iOS di Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 0aaece95effa468af5c906a8bd07e5b00ffa3df37b4e2cb296d64108efec94e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54047979"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Memecahkan masalah pendaftaran perangkat iOS di Microsoft Intune

Tinjau sumber daya yang tercantum di bawah ini untuk mengatasi masalah Anda sekarang. 
  
Beberapa pesan kesalahan umum dan langkah penyelesaian:
  
- **Jumlah Perangkat Tercapai** Pengguna telah mendaftarkan lebih banyak perangkat daripada batas perangkat. Tinjau dokumen ini [untuk menghapus perangkat](https://docs.microsoft.com/intune/devices-wipe) atau mengubah batas [perangkat](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Layanan ini tidak didukung. Tidak Ada Kebijakan Pendaftaran:** Apple Push Notification Service (APNS) harus dikonfigurasi atau diperbarui. Tinjau [dokumen](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) ini untuk mendapatkan instruksi tentang cara melakukannya. 
    
- **Tipe Lisensi Pengguna Tidak Valid atau Nama Pengguna Tidak Dikenali:** Pengguna harus diberi lisensi Intune atau EMS. Tinjau dokumen ini untuk menetapkan lisensi melalui: [Office Admin Atau](https://docs.microsoft.com/intune/licenses-assign) portal [Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Sumber daya tambahan untuk membantu mengatasi masalah Anda:
  
1. Gunakan [Portal Pemecahan Masalah Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) untuk mendiagnosis dan mengatasi kegagalan pendaftaran umum. Tinjau [dokumen ini](https://docs.microsoft.com/intune/help-desk-operators) untuk detail selengkapnya. 
    
2. Tinjau dokumen ini untuk daftar kesalahan umum yang mencegah pendaftaran dan resolusi untuk masing-masing: [Panduan pemecahan masalah](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) dan [Dokumen pemecahan masalah](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).
    
3. [Pelajari cara mendaftarkan perangkat iOS di Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

