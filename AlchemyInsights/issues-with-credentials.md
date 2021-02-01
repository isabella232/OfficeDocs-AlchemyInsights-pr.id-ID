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
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063678"
---
# <a name="issues-with-credentials"></a>Masalah dengan kredensial

[Platform identitas Microsoft dan aliran kredensial klien 2,0 OAuth](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) menjelaskan cara program langsung terhadap aliran hibah kredensial klien OAuth 2,0.

**Bagaimana cara mengelola kredensial kata sandi atau sertifikat aplikasi?**

Di Azure CLI, Anda bisa menggunakan [kredensial aplikasi AZ AD](https://docs.microsoft.com/cli/azure/ad/app/credential) untuk menghapus, membuat daftar, atau mereset kata sandi atau kredensial sertifikat aplikasi.

**Bagaimana cara pengguna mereset kata sandi mereka?**

Pengguna harus [mendaftar untuk mereset kata sandi layanan mandiri](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) sebelum mereka bisa mereset kata sandinya. Setelah pengguna mendaftar, mereka bisa mengikuti instruksi dalam artikel ini untuk mereset kata sandinya: [mereset kata sandi kantor atau sekolah Anda](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).

**Bagaimana cara pengguna mengubah kata sandi mereka?**

Pengguna dapat mengikuti langkah-langkah dalam artikel ini untuk mengubah kata sandinya: [cara mengubah kata sandi Anda](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).
Mereka juga bisa [mengelola kata sandi aplikasi untuk verifikasi dua langkah](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).

**Pengguna saya mendapatkan pesan kesalahan saat mengubah atau mengatur ulang kata sandi**

Link ini akan memberikan informasi tentang masalah umum yang dapat muncul saat pengguna mencoba mereset kata sandinya: [masalah umum dan solusinya](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Saya mengalami masalah mereset kata sandi pengguna**

- Pastikan Anda memiliki wewenang untuk mengatur ulang kata sandi. *Hanya global, kata sandi, dan administrator pengguna yang bisa mereset kata sandi pengguna.* Administrator global juga dapat mengatur ulang kata sandi administrator istimewa lainnya.

- Pastikan Anda memahami persyaratan Lisensi:

  - Anda harus memiliki setidaknya satu lisensi yang ditetapkan di organisasi Anda:
    - **Pengguna awan saja** -SKU Office 365 (O365) berbayar apa pun, atau Azure AD Basic
    - **Pengguna awan dan/atau di** tempat-Azure AD Premium P1 atau P2, mobilitas perusahaan + keamanan (EMS), atau mengamankan perusahaan produktif (SPE)
    - Untuk mempelajari selengkapnya tentang persyaratan lisensi, lihat [persyaratan lisensi untuk pengaturan ulang kata sandi layanan mandiri AZURE AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).
- Untuk mengatur ulang kata sandi pengguna, temukan pengguna di Azure AD. Lalu, pada bilah gambaran umum untuk pengguna tersebut, klik tombol "Atur ulang kata sandi."

**Tombol reset kata sandi berwarna abu-abu**

Anda tidak diizinkan untuk mereset kata sandi pengguna **ini** . *Hanya global, kata sandi, dan administrator pengguna yang bisa mereset kata sandi pengguna.* Administrator global juga dapat mengatur ulang kata sandi administrator istimewa lainnya.

**Saya tidak melihat Blade tata ulang kata sandi**

Anda tidak diberi wewenang untuk mengatur ulang kata sandi. *Hanya global, kata sandi, dan administrator pengguna yang bisa mereset kata sandi pengguna.* Administrator global juga dapat mengatur ulang kata sandi administrator istimewa lainnya.

**Saya tidak melihat Blade integrasi lokal dalam pengaturan ulang kata sandi**

- Bilah integrasi lokal hanya muncul di lingkungan hibrid-artinya Anda menggunakan tulis balik kata sandi untuk memanipulasi kata sandi pengguna di tempat.

- Anda tidak melihat pisau ini jika:

  - Anda tidak menggunakan tulis balik kata sandi
  - Ada masalah dengan instalasi/konektivitas tulis balik kata sandi Anda
  - Ada masalah dengan instalasi/konektivitas Azure AD Connect Anda
  - Untuk langkah pemecahan masalah lainnya untuk masalah dengan tulis balik kata sandi, lihat [memecahkan masalah tulis balik kata sandi](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Saya tidak tahu cara mengatur ulang kata sandi pengguna**

1. Masuk ke Azure Portal sebagai admin yang sesuai.
2. Masuk ke bilah **pengguna dan grup** , pilih **semua pengguna**.
3. Pilih pengguna dari daftar.
4. Untuk pengguna yang dipilih, pilih **gambaran umum**, lalu di bilah perintah, pilih **reset kata sandi**.
5. Pilih tombol **reset kata sandi** dan ikuti instruksi di layar.
    - Hanya mereset yang dilakukan melalui **Azure portal** mendukung tulis balik kata sandi.

**Saya mengatur ulang kata sandi pengguna lokal dari portal admin Office 365 atau aplikasi seluler Office 365 tapi pengguna masih belum dapat masuk**

Tulis balik kata sandi tidak didukung di portal ini. Atur ulang kata sandi pengguna lagi di portal Azure.
