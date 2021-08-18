---
title: Password Writeback is not working
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
ms.openlocfilehash: 679dea6d488cf74f51baee2b3b498dc64b95530e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324926"
---
# <a name="password-writeback-is-not-working"></a>Password Writeback is not working

**Saya mengalami masalah dalam mengonfigurasi kembali kata sandi**

- Password writeback is a premium feature.
- Pastikan bahwa Anda memahami persyaratan lisensi:
  - Anda harus memiliki setidaknya satu lisensi yang ditetapkan di organisasi Anda
  - **Pengguna hanya awan** - Semua Office 365 (O365) berbayar SKU, atau Azure AD Basic
  - **Pengguna lokal dan dan/atau** awan - Azure AD Premium P1 atau P2, Enterprise Mobility + Security (EMS), atau Secure Productive Enterprise (SPE)
    - Untuk mempelajari selengkapnya tentang persyaratan lisensi, lihat [Persyaratan lisensi untuk pengaturan ulang kata sandi layanan mandiri Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Anda memiliki setidaknya satu akun administrator dan satu akun pengguna uji dengan salah satu lisensi yang tepat.
- Anda harus menyambungkan Azure AD Koneksi ke Emulator Pengontrol Domain Utama agar alamat email dapat digunakan kembali. Anda bisa mengonfigurasi Azure AD Koneksi menggunakan Pengontrol Domain Utama  dengan mengklik kanan properti konektor sinkronisasi Direktori Aktif, lalu memilih konfigurasi **partisi direktori**. Dari sana, cari bagian **pengaturan koneksi pengontrol domain** dan periksa kotak yang berjudul hanya gunakan pengontrol domain **pilihan**.
    **Catatan**:Jika DC yang dipilih bukan emulator PDC, Azure AD Koneksi masih akan menghubungi PDC untuk menulis kembali kata sandi.
- Reset kata sandi telah dikonfigurasi dan diaktifkan di penyewa Anda. Untuk informasi selengkapnya, lihat [Memungkinkan pengguna mengatur ulang kata sandi Azure AD mereka.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)
- Pastikan bahwa akun administrator yang digunakan untuk mengaktifkan Penulisan Kata Sandi adalah akun administrator awan (dibuat di Azure AD bukan AD lokal)
- Anda memiliki penyebaran lokal ad tunggal atau multih hutan yang menjalankan Windows Server 2008 R2, Windows Server 2012, atau Windows Server 2012 R2 dengan paket layanan terbaru yang terinstal
- Anda telah menginstal alat Koneksi Azure AD dan telah menyiapkan lingkungan AD untuk sinkronisasi ke awan. Sebelum menguji kembali kata sandi, pastikan untuk menyelesaikan sinkronisasi penuh dan impor penuh terlebih dahulu dari AD dan Azure AD di Azure AD Koneksi.
- Untuk mempelajari selengkapnya, lihat cara melakukan sinkronisasi [penuh dan impor penuh di Azure AD Koneksi](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Saya mengalami masalah dengan konektivitas menulis kembali kata sandi**

1. Unduh dan aktifkan versi terbaru [Azure AD Koneksi](https://www.microsoft.com/download/details.aspx?id=47594)
2. Konfigurasi firewall: Alat Koneksi Azure AD (1.1.443 dan di atasnya) memerlukan **akses HTTPS** keluar ke:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Perbolehkan koneksi diam untuk tetap setidaknya 2-3 menit

**Saya masih mengalami masalah dengan kembalian kata sandi**

- Jika masih mengalami masalah, cobalah untuk menonaktifkan dan mengaktifkan kembali layanan penulisan kembali kata sandi di alat Koneksi Azure AD
- Untuk mempelajari selengkapnya, lihat cara [menonaktifkan dan mengaktifkan kembali penulisan kata sandi](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
