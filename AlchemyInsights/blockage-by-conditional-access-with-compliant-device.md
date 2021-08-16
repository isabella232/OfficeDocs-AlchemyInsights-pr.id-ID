---
title: Saya diblokir oleh Akses Bersyarat dengan perangkat yang memenuhi syarat
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
ms.openlocfilehash: 709749b1a62f2d9cdabfb3fe4b7538c22101d7109204d9163f6059336b817bf8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019151"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>Saya diblokir oleh Akses Bersyarat dengan perangkat yang memenuhi syarat

**Alat yang Sangat Direkomendasikan**

- [Alat Pemecah Masalah Registrasi Perangkat](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - Alat komprehensif yang membantu memecahkan masalah registrasi perangkat yang paling umum.
- [Skrip Uji Konektivitas Registrasi Perangkat](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - Alat yang digunakan untuk memastikan bahwa perangkat dapat mengakses titik akhir Registrasi Perangkat di bawah akun sistem.
- [Skrip Pembersihan Perangkat Azure AD](https://github.com/mzmaili/AzureADDeviceCleanup) - Alat yang digunakan untuk mencari dan mengelola perangkat basi di lingkungan Anda.

Berikut adalah beberapa alasan umum mengapa Akses Kondisional gagal pada perangkat  yang patuh atau mengapa pengguna Anda mungkin menerima Anda tidak bisa masuk ke sana dari sini saat pesan masuk ke sumber daya organisasi.

1. **Perangkat tidak berada dalam status perangkat yang diperlukan dengan MDM**:

Validasi bahwa perangkat terdaftar dengan penyedia MDM yang disetujui seperti Intune dan *ditandai sebagai memenuhi syarat.* Untuk informasi selengkapnya tentang Intune, lihat dokumen [ini](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment). Untuk pemahaman yang lebih baik tentang kepatuhan perangkat dan Intune, lihat menggunakan kebijakan kepatuhan untuk menetapkan aturan [bagi perangkat yang Anda kelola dengan Intune](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started). Jika Anda mengalami masalah saat mendaftarkan perangkat dengan Intune, temukan detail pemecahan masalah di [Memecahkan masalah pendaftaran perangkat di Microsoft](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune). Untuk dukungan Intune lebih lanjut, buat permintaan dukungan. Untuk melakukannya, kunjungi halaman Bantuan dan Dukungan [Intune](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).

2. **Perangkat tidak tergabung dalam jaringan organisasi:**

Untuk akses ke sumber daya organisasi, perangkat harus tersambung ke jaringan organisasi, baik melalui koneksi langsung atau jaringan privat virtual (VPN, Virtual Private Network), juga tergabung ke jaringan lokal atau Azure Active Directory. Untuk bergabung dengan perangkat kerja ke jaringan organisasi, [lihat Bergabung dengan perangkat kerja Anda ke jaringan organisasi Anda.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network) Untuk mendaftarkan perangkat pribadi/BYOD, [lihat Mendaftarkan perangkat pribadi Anda di jaringan organisasi Anda.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network)

- Untuk memvalidasi apakah perangkat telah bergabung dalam jaringan, Anda dapat mengikuti langkah-langkah untuk perangkat terdaftar di [sini atau](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) perangkat kerja di [sini](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined). Untuk lingkup masalah konektivitas jaringan Organisasi, ikuti panduan di bawah ini:

    1. Masuk untuk Windows akun kerja atau sekolah Anda, misalnya, alain@contoso.com.
    2. Koneksi ke jaringan organisasi Anda melalui VPN atau DirectAccess.
    3. Setelah tersambung, tekan tombol **Windows+L untuk** mengunci perangkat Anda.
    4. Buka kunci perangkat menggunakan akun kantor atau sekolah Anda, lalu coba akses kembali aplikasi atau layanan yang bermasalah.

Jika Anda melihat pesan **kesalahan Anda tidak bisa masuk ke sana dari** sini lagi, masalah mungkin berasal dari tempat lain.

3. **Sistem operasi tidak didukung:**

Pastikan Anda menjalankan versi sistem operasi yang didukung, termasuk:

- **klien Windows:** Windows 7 atau lebih baru

- **Windows Server:** Windows Server 2008 R2 atau yang lebih baru

- **macOS**: macOS X atau yang lebih baru

- **Android dan iOS**: Versi terbaru sistem operasi seluler Android dan iOS

4. **Browser web tidak didukung:**

Silakan temukan browser yang didukung di bawah ini. Untuk dukungan Chrome dengan Windows 1703 atau versi yang lebih baru, diperlukan Windows 10 Akun Pengguna. Untuk Edge 85+, pengguna harus masuk untuk menyampaikan informasi kepatuhan perangkat dengan benar. Untuk detail selengkapnya, lihat di [sini](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

- **Windows 10**: Microsoft Edge, Internet Explorer, Chrome
- **Windows 8 / 8.1**: Internet Explorer, Chrome
- **Windows 7**: Internet Explorer, Chrome
- **iOS**: Microsoft Edge, Browser yang Dikelola Intune, Safari
- **Android**: **Microsoft Edge**: Browser yang Dikelola Intune, Chrome
- **Windows Phone**: Microsoft Edge, Internet Explorer
- **Windows Server 2019:** Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016**: Internet Explorer
- **Windows Server 2012 R2**: Internet Explorer
- **Windows Server 2008 R2**: Internet Explorer
- **macOS**: Chrome, Safari

Temukan informasi selengkapnya tentang pesan **Tidak bisa masuk ke sana dan langkah-langkah** pemecahan masalah di [sini](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation).
