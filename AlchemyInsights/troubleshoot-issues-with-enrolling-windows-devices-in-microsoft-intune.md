---
title: Memecahkan masalah pendaftaran perangkat Windows di Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a456cc8f2336e6b902de0b7873cb233f4b846140
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51808974"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Memecahkan masalah pendaftaran perangkat Windows di Microsoft Intune

Tinjau sumber daya yang tercantum di bawah ini untuk mengatasi masalah Anda sekarang.
  
Beberapa pesan kesalahan umum dan langkah penyelesaian:
  
 **Perangkat lunak tidak dapat diinstal, 0x80cf4017:** Sertifikat akun Anda telah kedaluwarsa. Unduh ulang paket perangkat lunak Klien PC di Konsol Admin Intune. Tinjau dokumentasi ini untuk informasi selengkapnya.
  
 **Kode kesalahan 0x801c0003:** Kesalahan dapat terjadi pada skenario berikut:
  
-  Pengguna telah mendaftarkan lebih banyak perangkat daripada batas perangkat. Tinjau dokumen ini [untuk menghapus perangkat](https://docs.microsoft.com/intune/devices-wipe) atau mengubah batas [perangkat](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Pengguna dapat menggabungkan perangkat ke Azure AD" diatur ke "tidak ada." Atur ke semua atau pilih pengguna. Tinjau [dokumentasi ini](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) untuk informasi selengkapnya.

-  Perangkat tersebut sudah didaftarkan oleh pengguna lain. Jika demikian, hapus perangkat dari konsol Azure Intune atau hapus pendaftaran perangkat secara manual sebelum mencoba lagi.

-  Perangkatnya adalah Windows 10 Home. Hanya SKU Windows 10 Pro, Pendidikan, dan Perusahaan yang dapat bergabung dengan Azure Active Directory.

Sumber daya tambahan untuk membantu mengatasi masalah Anda:
  
-  Gunakan [Portal Pemecahan Masalah Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) untuk mendiagnosis dan mengatasi kegagalan pendaftaran umum. Tinjau [dokumen ini](https://docs.microsoft.com/intune/help-desk-operators) untuk detail selengkapnya.

-  Tinjau dokumen ini untuk melihat daftar kesalahan umum yang mencegah pendaftaran dan resolusi untuk masing-masing dokumen: [Panduan pemecahan masalah](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) dan Dokumen pemecahan [masalah.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)

[Pelajari cara mendaftarkan perangkat Windows di Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
