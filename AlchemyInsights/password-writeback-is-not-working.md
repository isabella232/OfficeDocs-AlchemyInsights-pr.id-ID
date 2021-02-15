---
title: Tulis balik kata sandi tidak berfungsi
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243368"
---
# <a name="password-writeback-is-not-working"></a>Tulis balik kata sandi tidak berfungsi

**Saya mengalami masalah saat mengonfigurasi tulis balik kata sandi**

- Tulis balik kata sandi adalah fitur Premium.
- Pastikan bahwa Anda memahami persyaratan Lisensi:
  - Anda harus memiliki setidaknya satu lisensi yang ditetapkan di organisasi Anda
  - **Pengguna awan saja** -SKU Office 365 (O365) berbayar apa pun, atau Azure AD Basic
  - **Pengguna awan dan/atau di** tempat-Azure AD Premium P1 atau P2, mobilitas perusahaan + keamanan (EMS), atau mengamankan perusahaan produktif (SPE)
    - Untuk mempelajari selengkapnya tentang persyaratan lisensi, lihat [persyaratan lisensi untuk pengaturan ulang kata sandi layanan mandiri AZURE AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Anda memiliki setidaknya satu akun administrator dan satu akun pengguna uji dengan salah satu lisensi yang sesuai.
- Anda harus menyambungkan Azure AD Connect ke emulator pengontrol domain utama untuk mencari tulis balik untuk bekerja. Anda bisa mengonfigurasi Azure AD Connect untuk menggunakan pengontrol domain utama dengan mengklik kanan pada **properti** konektor sinkronisasi direktori aktif, lalu memilih **Konfigurasikan partisi direktori**. Dari sana, Cari bagian **pengaturan koneksi pengontrol domain** dan centang kotak berjudul **hanya gunakan pengontrol domain pilihan**.
  > [!NOTE]
  > Jika DC pilihan bukan emulator PDC, Azure AD Connect masih akan menghubungi PDC untuk memasukkan kata sandi.
- Reset kata sandi telah dikonfigurasikan dan diaktifkan di penyewa Anda. Untuk informasi selengkapnya, lihat [mengaktifkan pengguna untuk mereset kata sandi AZURE AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).
- Pastikan bahwa akun administrator yang digunakan untuk mengaktifkan tulis balik kata sandi adalah akun administrator awan (dibuat di Azure AD not on-Premises AD)
- Anda memiliki satu atau beberapa Forest AD Deployment di tempat yang menjalankan Windows Server 2008 R2, Windows Server 2012, atau Windows Server 2012 R2 dengan paket layanan terbaru yang terinstal
- Anda memiliki alat Azure AD Connect yang terinstal dan Anda telah menyiapkan lingkungan iklan Anda untuk sinkronisasi ke awan. Sebelum menguji tulis balik kata sandi, pastikan bahwa Anda telah menyelesaikan impor lengkap dan sinkronisasi penuh baik dari AD maupun Azure AD di Azure AD Connect.
- Untuk mempelajari selengkapnya, Lihat cara melakukan [sinkronisasi penuh dan impor penuh di AZURE AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Saya mengalami masalah dengan konektivitas tulis balik kata sandi**

1. Mengunduh dan mengaktifkan versi terbaru [AZURE AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)
2. Konfigurasi firewall: alat Azure AD Connect (1.1.443 dan yang lebih baru) akan memerlukan akses **https keluar** ke:
    - passwordreset.microsoftonline.com
    - servicebus. Windows. Networks
3. Izinkan koneksi idle bertahan setidaknya selama 2-3 menit

**Saya masih mengalami masalah dengan tulis balik kata sandi**

- Jika Anda masih mengalami kesulitan, coba Nonaktifkan dan aktifkan kembali Layanan tulis balik kata sandi di alat Azure AD Connect
- Untuk mempelajari selengkapnya, Lihat cara [menonaktifkan dan mengaktifkan kembali tulis ulang kata sandi](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
