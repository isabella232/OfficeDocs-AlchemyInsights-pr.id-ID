---
title: Sinkronisasi kata sandi
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 3cdde086e535d2397b4d1a8a66903121a5217015ca055fb9f8d025b0842f044b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960838"
---
# <a name="password-synchronization"></a>Sinkronisasi kata sandi

**Sinkronisasi Hash Kata Sandi tidak berfungsi sama sekali**

Beberapa masalah umum yang dialami pelanggan ketika Sinkronisasi Hash Kata Sandi tidak berfungsi adalah:

- Akun Direktori Aktif yang digunakan oleh Azure AD Koneksi untuk berkomunikasi dengan Direktori Aktif di  tempat tidak diberikan Replika Perubahan **Direktori** dan Mereplikasi Perubahan Direktori Semua izin, yang diperlukan untuk sinkronisasi kata sandi - Anda perlu memperbaiki ini dengan memberi izin ini ke akun Direktori Aktif.
- Sinkronisasi hash kata sandi dinonaktifkan setelah administrator mengubah metode  User Sign-In dari Sinkronisasi Kata Sandi ke opsi lain seperti Federasi dengan **AD FS** dalam panduan Koneksi Azure AD - Anda dapat memperbaikinya dengan mengaktifkan kembali fitur sinkronisasi **hash** kata sandi dalam panduan Koneksi Azure AD.
- Masalah konektivitas dengan Direktori Aktif di tempat. Misalnya, beberapa pengontrol domain tidak dapat diakses oleh Azure AD [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) Koneksi, atau port yang diperlukan diblokir oleh Firewall - Anda perlu memperbaikinya dengan memastikan bahwa konektivitas antara server azure AD Koneksi dan Direktori Aktif lokal berfungsi dengan benar.
- Server Azure AD Koneksi saat ini sedang dalam mode pengaturan, yang akan mengakibatkan server tidak dapat menggunakan hash kata sandi - Untuk memecahkan masalah, ikuti langkah-langkah yang diuraikan di bagian Memecahkan masalah sinkronisasi kata sandi dengan sinkronisasi Azure AD Koneksi - Tidak ada kata sandi yang [disinkronkan.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

**Sinkronisasi Hash Kata Sandi tidak berfungsi untuk beberapa pengguna saya**

1. Jika Anda menyadari bahwa hash kata sandi tidak disinkronkan untuk pengguna, gunakan tugas pemecahan masalah di Azure AD Koneksi menyelidiki dan mengatasi masalah tersebut.  Lakukan tugas-tugas berikut:

    a. [Menjalankan tugas pemecahan masalah dalam panduan](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Menggunakan cmdlet pemecahan masalah untuk menyelidiki masalah sinkronisasi hash kata sandi untuk penggunaan tertentu](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. Objek Pengguna Direktori Aktif di tempat diaktifkan untuk Pengguna harus **mengubah kata sandi pada opsi masuk** berikutnya. Saat opsi ini diaktifkan, pengguna diberikan kata sandi sementara dan akan diminta untuk mengubah kata sandi pada saat masuk berikutnya. Azure AD Koneksi tidak menyinkronkan kata sandi sementara ke Azure AD.

Untuk mengatasi masalah di atas, lakukan salah satu tugas berikut ini:

- Mintalah pengguna untuk masuk ke aplikasi lokal (misalnya, desktop Windows) dan mengubah kata sandi. Kata sandi baru akan disinkronkan ke Azure AD.
- Mempunyai administrator yang memperbarui kata sandi pengguna tanpa mengaktifkan opsi Pengguna harus mengubah kata sandi pada saat masuk berikutnya **,** dan bagikan kata sandi yang baru dengan pengguna.

3. Objek Pengguna Direktori Aktif di tempat tidak dikonfigurasi **dengan benar untuk sinkronisasi** objek atau sinkronisasi kata sandi. Untuk memecahkan masalah ini, ikuti langkah-langkah yang diuraikan dalam Memecahkan masalah sinkronisasi [hash kata sandi dengan sinkronisasi Koneksi Azure AD.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)







