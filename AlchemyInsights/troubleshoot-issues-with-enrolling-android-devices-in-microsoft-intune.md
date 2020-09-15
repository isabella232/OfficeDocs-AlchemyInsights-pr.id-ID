---
title: Memecahkan masalah dengan mendaftarkan perangkat Android di Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689957"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Memecahkan masalah dengan mendaftarkan perangkat Android di Microsoft Intune

Tinjau sumber daya yang tercantum di bawah ini untuk mengatasi masalah Anda sekarang.
  
Beberapa masalah umum dan langkah pemecahan masalah:
  
 **Kesalahan perangkat tidak dienkripsi di portal perusahaan:** Versi Android yang lebih baru, terutama diawali dengan v 7.0, memerlukan kode akses untuk memastikan bahwa perangkat Anda dienkripsi penuh. Solusi umum adalah untuk mengaktifkan pin startup atau mengenkripsi penuh perangkat. Tinjau [dokumen ini](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) untuk informasi selengkapnya.
  
 **Perangkat gagal Check-in dengan layanan Intune atau ditampilkan sebagai "tidak sehat" di konsol admin Intune:** Beberapa perangkat Samsung 4,4 dan 5,5 mungkin tidak memeriksa layanan. Ada 3 solusi yang memungkinkan untuk masalah ini:
  
1. Buka aplikasi Intune Company portal secara manual, yang akan memulai sinkronisasi perangkat secara otomatis.

2. Perbarui perangkat ke Android 6,0 atau yang lebih tinggi.

3. Nonaktifkan Samsung Smart Manager dari mengelola portal perusahaan Intune. Tinjau [dokumen ini](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) untuk detail lebih lanjut tentang masalah dan resolusi ini.

 **Lisensi pengguna ketik** **nama pengguna tidak valid atau tidak dikenali kesalahan:** pengguna harus diberi lisensi Intune atau EMS. Tinjau dokumen ini untuk menetapkan lisensi melalui: Pusat admin Office atau Azure portal.
  
Sumber daya tambahan untuk membantu mengatasi masalah Anda:
  
1. Gunakan [portal pemecahan masalah Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) untuk mendiagnosis dan mengatasi kegagalan pendaftaran umum. Tinjau [dokumen ini](https://docs.microsoft.com/intune/help-desk-operators) untuk detail selengkapnya.

2. Tinjau [dokumen ini](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) untuk daftar kesalahan umum yang mencegah pendaftaran dan resolusi untuk masing-masing.

3. [Pelajari cara mendaftarkan perangkat Android di Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
