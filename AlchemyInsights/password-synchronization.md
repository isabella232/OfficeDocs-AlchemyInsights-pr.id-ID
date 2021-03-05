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
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482037"
---
# <a name="password-synchronization"></a>Sinkronisasi kata sandi

**Sinkronisasi hash kata sandi tidak berfungsi sama sekali**

Beberapa masalah umum yang dihadapi pelanggan ketika sinkronisasi hash kata sandi tidak berfungsi:

- Akun direktori aktif yang digunakan oleh Azure AD Connect untuk berkomunikasi dengan direktori aktif di tempat tidak diberikan **replikasi perubahan direktori** dan **replikasi perubahan direktori semua** izin, yang diperlukan untuk sinkronisasi kata sandi-Anda perlu memperbaikinya dengan memberikan izin ini ke akun direktori aktif.
- Sinkronisasi hash kata sandi dinonaktifkan setelah administrator mengubah metode Sign-In pengguna dari **sinkronisasi kata sandi** ke opsi lain seperti **Federasi dengan AD FS** dalam panduan Azure AD Connect-Anda bisa memperbaikinya dengan mengaktifkan ulang fitur **sinkronisasi hash kata sandi** dalam panduan Azure AD Connect.
- Masalah konektivitas dengan direktori aktif di tempat. Misalnya, beberapa pengontrol domain tidak dapat diakses oleh Azure AD Connect, atau port yang [diperlukan](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) diblokir oleh firewall-Anda harus memperbaikinya dengan memastikan bahwa konektivitas antara server Azure AD Connect dan direktori aktif di tempat berfungsi dengan benar.
- Server Azure AD Connect sedang berada dalam mode pementasan, yang akan menyebabkan server tidak bisa menggunakan hash kata sandi-untuk memecahkan masalah, ikuti langkah-langkah yang diuraikan dalam [memecahkan masalah sinkronisasi kata sandi dengan sinkronisasi AZURE AD Connect-tidak ada kata sandi yang disinkronkan](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).

**Sinkronisasi hash kata sandi tidak berfungsi untuk beberapa pengguna saya**

1. Jika Anda melihat bahwa hash kata sandi tidak disinkronkan untuk pengguna, gunakan tugas **pemecahan masalah** di Azure AD Connect untuk menyelidiki dan mengatasi masalah tersebut. Melakukan tugas berikut:

    untuk. [Menjalankan tugas pemecahan masalah dalam panduan](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Menggunakan cmdlet pemecahan masalah untuk menyelidiki masalah sinkronisasi hash kata sandi untuk penggunaan tertentu](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. Objek pengguna Active Directory lokal diaktifkan untuk opsi **pengguna harus mengubah kata sandi pada logon berikutnya** . Ketika opsi ini diaktifkan, pengguna diberi kata sandi sementara dan akan diminta untuk mengubah kata sandi pada logon berikutnya. Azure AD Connect tidak menyinkronkan kata sandi sementara ke Azure AD.

Untuk mengatasi masalah di atas, lakukan salah satu tugas berikut:

- Minta pengguna untuk masuk ke aplikasi di tempat (misalnya, desktop Windows) dan ubah kata sandinya. Kata sandi baru akan disinkronkan ke Azure AD.
- Memiliki administrator yang memperbarui kata sandi pengguna tanpa mengaktifkan opsi **pengguna harus mengubah kata sandi pada logon berikutnya**, dan berbagi kata sandi baru dengan pengguna.

3. Objek pengguna direktori aktif lokal **tidak dikonfigurasi dengan benar** untuk sinkronisasi objek atau sinkronisasi kata sandi. Untuk memecahkan masalah ini, ikuti langkah-langkah yang diuraikan dalam [memecahkan sinkronisasi hash kata sandi dengan sinkronisasi AZURE AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).







