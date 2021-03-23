---
title: Saya mendapatkan diblokir oleh akses bersyarat dengan perangkat yang memenuhi syarat
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 240bd25f4d62505202c8cd7ceabe4c1cd3d5c0b5
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035996"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>Saya mendapatkan diblokir oleh akses bersyarat dengan perangkat yang memenuhi syarat

**Alat yang sangat direkomendasikan**

- [Alat pemecah masalah registrasi perangkat](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) -alat komprehensif yang membantu memecahkan masalah pendaftaran perangkat yang paling umum.
- [Skrip konektivitas registrasi perangkat uji](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) -alat yang digunakan untuk memastikan bahwa perangkat dapat mengakses titik akhir pendaftaran perangkat di bawah akun sistem.
- [Skrip pembersihan perangkat AZURE AD](https://github.com/mzmaili/AzureADDeviceCleanup) -alat yang digunakan untuk mencari dan mengelola perangkat yang basi di lingkungan Anda.

Berikut adalah beberapa alasan umum mengapa akses bersyarat mungkin gagal untuk perangkat yang sesuai atau mengapa pengguna Anda mungkin menerima pesan tidak **bisa masuk ke sana dari sini** selama permintaan masuk ke sumber daya organisasi.

1. **Perangkat tidak berada dalam status perangkat yang diperlukan dengan Mdm**:

Memvalidasi bahwa perangkat didaftarkan dengan penyedia MDM yang disetujui seperti Intune dan *ditandai sebagai patuh*. Untuk informasi selengkapnya tentang Intune, lihat [dokumen](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment)ini. Untuk pemahaman yang lebih baik tentang kepatuhan perangkat dan Intune, lihat [menggunakan kebijakan kepatuhan untuk mengatur aturan untuk perangkat yang Anda Kelola dengan Intune](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started). Jika Anda mengalami masalah saat mendaftarkan perangkat dengan Intune, temukan detail pemecahan masalah [dalam menyelesaikan masalah pendaftaran perangkat di Microsoft](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune). Untuk dukungan Intune lebih lanjut, buat permintaan dukungan. Untuk melakukannya, kunjungi [halaman bantuan dan dukungan Intune](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).

2. **Perangkat tidak digabungkan ke jaringan organisasi**:

Untuk akses ke sumber daya organisasi, perangkat harus tersambung ke jaringan organisasi, baik melalui koneksi langsung maupun jaringan privat virtual (VPN), dan juga bergabung ke di tempat atau direktori aktif Azure. Untuk bergabung dengan perangkat kerja ke jaringan organisasi, lihat [bergabung dengan perangkat kerja Anda ke jaringan organisasi Anda](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network). Untuk mendaftarkan perangkat pribadi/BYOD, lihat [mendaftarkan perangkat pribadi Anda di jaringan organisasi Anda](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network).

- Untuk memvalidasi Apakah perangkat telah bergabung dalam jaringan, Anda bisa mengikuti langkah-langkah untuk perangkat terdaftar [di sini](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) atau perangkat kantor [di sini](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined). Untuk lingkup masalah konektivitas jaringan organisasi, ikuti panduan di bawah ini:

    1. Masuk ke Windows menggunakan akun kantor atau sekolah Anda, misalnya, alain@contoso.com.
    2. Sambungkan ke jaringan organisasi Anda melalui VPN atau DirectAccess.
    3. Setelah Anda tersambung, tekan **tombol logo Windows + L** untuk mengunci perangkat Anda.
    4. Buka perangkat Anda menggunakan akun kantor atau sekolah, lalu Cobalah untuk mengakses aplikasi atau layanan bermasalah lagi.

Jika Anda melihat pesan kesalahan **Anda tidak dapat masuk ke sana dari sini** , masalah mungkin terjadi di tempat lain.

3. **Sistem operasi tidak didukung**:

Pastikan Anda menjalankan versi sistem operasi yang didukung, termasuk:

- **Klien Windows**: Windows 7 atau yang lebih baru

- **Server Windows**: windows Server 2008 R2 atau yang lebih baru

- **MacOS**: MacOS X atau yang lebih baru

- **Android dan IOS**: versi terbaru sistem operasi seluler Android dan IOS

4. **Browser web tidak didukung**:

Temukan browser yang didukung di bawah ini. Untuk dukungan Chrome dengan Windows 1703 atau versi yang lebih baru, ekstensi akun Windows 10 diperlukan. Untuk Edge 85 +, pengguna harus masuk untuk mengirimkan informasi kepatuhan perangkat dengan benar. Untuk detail selengkapnya, lihat [di sini](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

- **Windows 10**: Microsoft Edge, Internet Explorer, Chrome
- **Windows 8/8,1**: Internet Explorer, Chrome
- **Windows 7**: Internet Explorer, Chrome
- **IOS**: Microsoft Edge, Intune Managed browser, Safari
- **Android**: **Microsoft Edge**: Intune Managed browser, Chrome
- **Windows Phone**: Microsoft Edge, Internet Explorer
- **Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016**: Internet Explorer
- **Windows Server 2012 R2**: Internet Explorer
- **Windows Server 2008 R2**: Internet Explorer
- **macOS**: Chrome, Safari

Temukan informasi selengkapnya **tentang pesan dan** langkah pemecahan masalah di [sini](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation).
