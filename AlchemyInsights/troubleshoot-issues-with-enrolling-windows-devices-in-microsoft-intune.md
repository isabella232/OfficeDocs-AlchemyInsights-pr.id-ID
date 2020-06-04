---
title: Memecahkan masalah dengan mendaftarkan perangkat Windows di Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665835"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Memecahkan masalah dengan mendaftarkan perangkat Windows di Microsoft Intune

Tinjau sumber daya yang tercantum di bawah ini untuk menyelesaikan masalah Anda sekarang.
  
Beberapa pesan error dan langkah resolusi umum:
  
 **Perangkat lunak tidak dapat diinstal, 0x80cf4017:** Sertifikat akun Anda telah kedaluwarsa. Download ulang paket perangkat lunak PC client di konsol admin Intune. Tinjau dokumentasi ini untuk informasi lebih lanjut.
  
 **Kode galat 0x801c0003:** Galat dapat terjadi dalam skenario berikut:
  
-  Pengguna memiliki lebih banyak perangkat yang terdaftar daripada batas perangkat. Tinjau dokumen ini untuk [menghapus perangkat](https://docs.microsoft.com/intune/devices-wipe) atau [mengubah batas perangkat](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Pengguna dapat bergabung dengan perangkat ke Azure AD" diatur ke "none". Atur ke semua atau pilih pengguna. Tinjau [dokumentasi ini](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) untuk informasi lebih lanjut.

-  Perangkat telah didaftarkan oleh pengguna lain. Jika demikian, Hapus perangkat dari konsol Intune Azure atau secara manual membatalkan pendaftaran perangkat sebelum mencoba lagi.

-  Perangkat ini adalah Windows 10 Home. Hanya Windows 10 Pro, pendidikan, dan Enterprise SKU yang dapat bergabung dengan Azure Active Directory.

Sumber daya tambahan untuk membantu menyelesaikan masalah Anda:
  
-  Gunakan [Intune pemecahan masalah portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) untuk mendiagnosis dan menyelesaikan umum kegagalan pendaftaran. Tinjau [dokumen ini](https://docs.microsoft.com/intune/help-desk-operators) untuk detail selengkapnya.

-  Tinjau dokumen ini untuk daftar kesalahan umum yang mencegah pendaftaran dan resolusi untuk masing-masing: [panduan pemecahan](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) masalah dan [pemecahan masalah dokumen](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Pelajari cara mendaftarkan perangkat Windows di Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
