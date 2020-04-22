---
title: Memecahkan masalah dengan mendaftarkan perangkat Android di Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759623"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Memecahkan masalah dengan mendaftarkan perangkat Android di Microsoft Intune

Tinjau sumber daya yang tercantum di bawah ini untuk menyelesaikan masalah Anda sekarang.
  
Beberapa masalah umum dan langkah penyelesaian:
  
 **Perangkat tidak dienkripsi kesalahan di portal perusahaan:** Versi Android yang lebih baru, khususnya dimulai dengan v 7.0, memerlukan kode sandi mulai untuk memastikan perangkat Anda dienkripsi sepenuhnya. Solusi umum adalah untuk mengaktifkan pin startup atau sepenuhnya mengenkripsi perangkat. Tinjau [dokumen ini](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) untuk informasi lebih lanjut.
  
 **Perangkat gagal untuk Check-in dengan layanan Intune atau menampilkan sebagai "tidak sehat" di konsol admin Intune:** Beberapa Samsung 4,4 dan perangkat 5,5 mungkin tidak memeriksa ke dalam layanan. Ada 3 kemungkinan solusi untuk masalah ini:
  
1. Buka aplikasi portal perusahaan Intune secara manual, yang akan memulai sinkronisasi perangkat secara otomatis.

2. Perbarui perangkat ke Android 6,0 atau versi yang lebih baru.

3. Nonaktifkan Samsung Smart Manager mengelola Intune portal perusahaan. Tinjau [dokumen ini](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) untuk detail lebih lanjut tentang masalah dan resolusi ini.

 **Jenis lisensi pengguna tidak valid** atau **nama pengguna tidak dikenali galat:** pengguna harus ditetapkan lisensi Intune atau EMS. Tinjau dokumen ini untuk menetapkan lisensi melalui: Pusat admin Office atau Azure portal.
  
Sumber daya tambahan untuk membantu menyelesaikan masalah Anda:
  
1. Gunakan [Intune pemecahan masalah portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) untuk mendiagnosis dan menyelesaikan umum kegagalan pendaftaran. Tinjau [dokumen ini](https://docs.microsoft.com/intune/help-desk-operators) untuk detail selengkapnya.

2. Tinjau [dokumen ini](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) untuk daftar kesalahan umum yang mencegah pendaftaran dan resolusi untuk masing-masing.

3. [Pelajari cara mendaftarkan perangkat Android di Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
