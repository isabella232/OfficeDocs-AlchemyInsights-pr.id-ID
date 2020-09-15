---
title: Memecahkan masalah dengan perangkat Windows yang didaftarkan di Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658881"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Memecahkan masalah dengan perangkat Windows yang didaftarkan di Microsoft Intune

Tinjau sumber daya yang tercantum di bawah ini untuk mengatasi masalah Anda sekarang.
  
Beberapa langkah pemecahan masalah dan pesan kesalahan umum:
  
 **Perangkat lunak tidak dapat diinstal, 0x80cf4017:** Sertifikat akun Anda telah kedaluwarsa. Mengunduh ulang paket perangkat lunak klien PC di konsol admin Intune. Tinjau dokumentasi ini untuk informasi selengkapnya.
  
 **Kode kesalahan 0x801c0003:** Kesalahan bisa terjadi dalam skenario berikut ini:
  
-  Pengguna memiliki lebih banyak perangkat yang terdaftar dibandingkan batas perangkat. Tinjau dokumen ini untuk [menghapus perangkat](https://docs.microsoft.com/intune/devices-wipe) atau [mengubah batas perangkat](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Pengguna bisa bergabung dengan perangkat ke Azure AD" diatur ke "none." Atur ke semua atau pilih pengguna. Tinjau [dokumentasi ini](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) untuk informasi selengkapnya.

-  Perangkat telah didaftarkan oleh pengguna lain. Jika demikian, Hapus perangkat dari konsol Azure Intune atau Batalkan pendaftaran perangkat secara manual sebelum mencoba lagi.

-  Perangkat tersebut adalah Windows 10 Home. Hanya Windows 10 Pro, pendidikan dan SKU Enterprise yang bisa bergabung dengan Azure Active Directory.

Sumber daya tambahan untuk membantu mengatasi masalah Anda:
  
-  Gunakan [portal pemecahan masalah Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) untuk mendiagnosis dan mengatasi kegagalan pendaftaran umum. Tinjau [dokumen ini](https://docs.microsoft.com/intune/help-desk-operators) untuk detail selengkapnya.

-  Tinjau dokumen ini untuk daftar kesalahan umum yang mencegah pendaftaran dan resolusi untuk masing-masing: [panduan pemecahan](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) masalah dan dokumen [pemecahan masalah](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Pelajari cara mendaftarkan perangkat Windows di Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
