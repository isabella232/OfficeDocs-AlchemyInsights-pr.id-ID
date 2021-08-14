---
title: Masalah dengan kredensial
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
- "9004330"
- "7723"
ms.openlocfilehash: 975d4850c1ecffae786dd19b7f4363e0c95378cff4f3ae6bb1968af33ef810b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986822"
---
# <a name="issues-with-credentials"></a>Masalah dengan kredensial

platform identitas Microsoft dan aliran kredensial klien [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) menjelaskan cara memprogram secara langsung terhadap aliran kredensial klien OAuth 2.0.

**Bagaimana cara mengelola kata sandi atau kredensial sertifikat aplikasi?**

Di Azure CLI, Anda dapat menggunakan [kredensial aplikasi az ad](https://docs.microsoft.com/cli/azure/ad/app/credential) untuk menghapus, mencantumkan, atau mengatur ulang kata sandi atau kredensial sertifikat aplikasi.

**Bagaimana cara pengguna saya mengatur ulang kata sandi mereka?**

Pengguna harus mendaftarkan [pengaturan ulang kata sandi layanan mandiri sebelum](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) mereka dapat mengatur ulang kata sandi mereka. Setelah pengguna mendaftar, mereka dapat mengikuti instruksi dalam artikel ini untuk mengatur ulang kata sandi mereka: [Mengatur ulang kata sandi kantor atau sekolah Anda](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).

**Bagaimana pengguna saya mengubah kata sandi mereka?**

Pengguna dapat mengikuti langkah-langkah dalam artikel ini untuk mengubah kata sandinya: [Cara mengubah kata sandi.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)
Mereka juga dapat [Mengelola kata sandi aplikasi untuk verifikasi dua langkah.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)

**Pengguna saya mendapatkan kesalahan ketika mengubah atau mengatur ulang kata sandi mereka**

Link ini akan menyediakan informasi tentang masalah umum yang bisa terjadi saat pengguna mencoba untuk mereset kata sandi mereka: [Masalah umum dan solusinya](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Saya mengalami masalah saat mengatur ulang kata sandi pengguna**

- Pastikan Anda diizinkan untuk mengatur ulang kata sandi. *Hanya administrator global, kata sandi, dan pengguna yang bisa mereset kata sandi pengguna.* Administrator global juga dapat mengatur ulang kata sandi administrator istimewa lainnya.

- Pastikan Anda memahami persyaratan lisensi:

  - Anda setidaknya harus memiliki satu lisensi yang ditetapkan di organisasi:
    - **Pengguna awan saja** - Semua Office 365 (O365) berbayar SKU, atau Azure AD Basic
    - **Pengguna lokal dan dan/atau** awan - Azure AD Premium P1 atau P2, Enterprise Mobility + Security (EMS), atau Secure Productive Enterprise (SPE)
    - Untuk mempelajari selengkapnya tentang persyaratan lisensi, lihat [Persyaratan lisensi untuk pengaturan ulang kata sandi layanan mandiri Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Untuk mengatur ulang kata sandi pengguna, temukan pengguna di Azure AD. Lalu, pada blade gambaran umum untuk pengguna tersebut, klik tombol "reset kata sandi".

**Tombol reset kata sandi berwarna abu-abu**

Anda tidak diizinkan untuk mengatur ulang **kata** sandi pengguna ini. *Hanya administrator global, kata sandi, dan pengguna yang bisa mereset kata sandi pengguna.* Administrator global juga dapat mengatur ulang kata sandi administrator istimewa lainnya.

**Saya tidak melihat kata sandi mereset blade**

Anda tidak diizinkan untuk mengatur ulang kata sandi. *Hanya administrator global, kata sandi, dan pengguna yang bisa mereset kata sandi pengguna.* Administrator global juga dapat mengatur ulang kata sandi administrator istimewa lainnya.

**Saya tidak melihat blade integrasi di tempat dalam pengaturan ulang kata sandi**

- Blade integrasi di tempat hanya muncul di lingkungan hibrid - artinya Anda menggunakan kembali kata sandi untuk memanipulasi kata sandi pengguna lokal.

- Anda tidak melihat blade ini jika:

  - Anda tidak menggunakan kembali kata sandi
  - Ada masalah dengan penginstalan/konektivitas penulisan kata sandi
  - Ada masalah dengan instalasi/konektivitas Azure AD Koneksi
  - Untuk langkah pemecahan masalah selengkapnya terkait masalah dengan kembali menulis kata sandi, lihat Memecahkan [masalah penulisan kembali kata sandi](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Saya tidak tahu cara mengatur ulang kata sandi pengguna**

1. Masuk ke portal Azure sebagai admin yang tepat.
2. Buka blade **Pengguna dan grup,** pilih **Semua Pengguna.**
3. Pilih pengguna dari daftar.
4. Untuk pengguna yang dipilih, pilih **Gambaran Umum**, lalu di bilah perintah, pilih Reset **kata sandi**.
5. Pilih tombol **Atur ulang** kata sandi dan ikuti instruksi di layar.
    - Hanya mereset yang dilakukan melalui **portal Azure** mendukung penulisan kembali kata sandi.

**Saya mereset kata sandi pengguna di tempat dari portal Office 365 Admin atau Office 365 seluler tapi pengguna masih tidak bisa masuk**

Password Writeback tidak didukung di portal ini. Reset kembali kata sandi pengguna di portal Azure.
