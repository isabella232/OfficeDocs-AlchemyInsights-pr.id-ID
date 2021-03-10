---
title: Masalah mereset kata sandi
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694378"
---
# <a name="problems-resetting-password"></a>Masalah mereset kata sandi

Berikut ini adalah beberapa masalah yang mungkin Anda hadapi saat mereset kata sandi dan solusi yang memungkinkan:

**Saya mengalami masalah dengan penyetelan ulang kata sandi yang tidak tercakup dalam kategori lain**

- Pastikan Anda memiliki wewenang untuk mengatur ulang kata sandi. Hanya global, kata sandi, dan administrator pengguna yang bisa mereset kata sandi pengguna. Administrator global juga dapat mengatur ulang kata sandi administrator istimewa lainnya.
- Pastikan bahwa Anda memahami persyaratan Lisensi:
    - Anda harus memiliki setidaknya satu lisensi yang ditetapkan di organisasi Anda
        - Pengguna awan saja-SKU Office 365 (O365) berbayar apa pun, atau Azure AD Basic
        - Pengguna awan dan/atau di tempat-Azure AD Premium P1 atau P2, mobilitas perusahaan + keamanan (EMS), atau mengamankan perusahaan produktif (SPE)
        - Untuk membaca selengkapnya tentang persyaratan lisensi Lihat artikel [persyaratan lisensi untuk reset kata sandi layanan mandiri AZURE AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).

**Saya mengalami masalah dalam menguji kebijakan penyetelan ulang kata sandi yang saya atur**

- Kebijakan yang baru diterapkan dapat memakan waktu beberapa menit untuk mengulangi seluruh pusat data dan titik akhir. Jarak fisik dari pusat data juga akan mempengaruhi seberapa cepat perubahan diterapkan.
- Uji dengan pengguna akhir, bukan administrator, dan percobaan dengan sekelompok kecil pengguna. Kebijakan yang dikonfigurasi di Azure portal hanya berlaku untuk pengguna akhir, bukan administrator. Microsoft memberlakukan kebijakan penyetelan ulang kata sandi default yang kuat untuk setiap peran administrator Azure (contoh: administrator global, administrator Meja bantuan, administrator kata sandi, dsb.)
    - Pelajari selengkapnya tentang [kebijakan untuk administrator](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).

**Saya ingin menggunakan pengaturan ulang kata sandi tapi saya tidak ingin membuat pengguna saya mendaftarkan Info keamanan tambahan**

Pra-isi data untuk pengguna Anda sehingga mereka tidak harus! -Sebagai administrator Anda bisa mengatur properti telepon dan email untuk pengguna Anda sebelum meluncurkan pengaturan ulang kata sandi ke organisasi Anda. Anda dapat melakukan ini menggunakan API, PowerShell, atau Azure AD Connect. Informasi selengkapnya di sini:
- [Menyebarkan penyetelan ulang kata sandi tanpa mengharuskan pengguna untuk mendaftar](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Data apa yang digunakan oleh reset kata sandi](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Tombol reset kata sandi berwarna abu-abu**

Anda tidak diizinkan untuk mereset kata sandi pengguna ini. Hanya global, kata sandi, dan administrator pengguna yang bisa mereset kata sandi pengguna. Administrator global juga dapat mengatur ulang kata sandi administrator istimewa lainnya.

**Saya tidak melihat Blade tata ulang kata sandi**

Anda tidak diberi wewenang untuk mengatur ulang kata sandi. Hanya global, kata sandi, dan administrator pengguna yang bisa mereset kata sandi pengguna. Administrator global juga dapat mengatur ulang kata sandi administrator istimewa lainnya.

**Saya tidak melihat Blade integrasi lokal dalam pengaturan ulang kata sandi**

- Bilah integrasi lokal hanya muncul di lingkungan hibrid-artinya Anda menggunakan tulis balik kata sandi untuk memanipulasi kata sandi pengguna di tempat.
- Anda tidak melihat pisau ini jika:
    - Anda tidak menggunakan tulis balik kata sandi
    - Ada masalah dengan instalasi/konektivitas tulis balik kata sandi Anda
    - Ada masalah dengan instalasi/konektivitas Azure AD Connect Anda
    - Untuk langkah pemecahan masalah lainnya untuk masalah dengan tulis balik kata sandi, lihat bagian [memecahkan masalah tulis balik kata sandi](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Saya tidak tahu cara mengatur ulang kata sandi pengguna**

1. Masuk ke Azure Portal sebagai admin yang sesuai.
1. Masuk ke bilah pengguna dan grup, pilih **semua pengguna**.
1. Pilih pengguna dari daftar.
1. Untuk pengguna yang dipilih, pilih **gambaran umum**, lalu di bilah perintah, klik **reset kata sandi**.
1. Ikuti instruksi di layar.
    - Hanya mereset yang dilakukan melalui Azure portal mendukung tulis balik kata sandi.

**Saya mengatur ulang kata sandi pengguna lokal dari portal admin Office 365 atau aplikasi seluler Office 365 tapi pengguna masih belum dapat masuk**

Tulis balik kata sandi tidak didukung di portal ini. Mengatur ulang kata sandi pengguna lagi di portal Azure-portal.azure.com

