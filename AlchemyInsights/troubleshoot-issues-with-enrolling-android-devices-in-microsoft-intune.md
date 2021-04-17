---
title: Memecahkan masalah pendaftaran perangkat Android di Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 08620a44dcf693482c65ff05e19f11870f67afbe
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830945"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Memecahkan masalah pendaftaran perangkat Android di Microsoft Intune

Tinjau sumber daya yang tercantum di bawah ini untuk mengatasi masalah Anda sekarang.
  
Beberapa masalah umum dan langkah-langkah penyelesaian:
  
 **Kesalahan Perangkat tidak Dienkripsi di Portal Perusahaan:** Versi android yang lebih baru, terutama yang dimulai dengan v7.0, memerlukan kode akses mulai untuk memastikan bahwa perangkat Anda dienkripsi sepenuhnya. Solusi umum adalah mengaktifkan pin mulai atau mengenkripsi perangkat sepenuhnya. Tinjau [dokumen ini](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) untuk informasi selengkapnya.
  
 **Perangkat tidak dapat masuk dengan layanan Intune atau ditampilkan sebagai "Tidak sehat" di konsol admin Intune:** Beberapa perangkat Samsung 4.4 dan 5.5 mungkin tidak masuk ke layanan. Ada 3 solusi yang memungkinkan untuk masalah ini:
  
1. Buka aplikasi Intune Company Portal secara manual, yang akan memulai sinkronisasi perangkat secara otomatis.

2. Perbarui perangkat ke Android 6.0 atau yang lebih tinggi.

3. Nonaktifkan Samsung Smart Manager dari mengelola Portal Perusahaan Intune. Tinjau [dokumen ini](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) untuk detail selengkapnya mengenai masalah dan resolusi ini.

 **Kesalahan Tipe Lisensi Pengguna** Tidak Valid atau Nama Pengguna Tidak **Dikenali:** Pengguna perlu diberi lisensi Intune atau EMS. Tinjau dokumen ini untuk menetapkan lisensi melalui: Pusat Admin Office atau portal Azure.
  
Sumber daya tambahan untuk membantu mengatasi masalah Anda:
  
1. Gunakan [Portal Pemecahan Masalah Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) untuk mendiagnosis dan mengatasi kegagalan pendaftaran umum. Tinjau [dokumen ini](https://docs.microsoft.com/intune/help-desk-operators) untuk detail selengkapnya.

2. Tinjau [dokumen](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) ini untuk daftar kesalahan umum yang mencegah pendaftaran dan resolusi untuk masing-masing.

3. [Pelajari cara mendaftarkan perangkat Android di Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
