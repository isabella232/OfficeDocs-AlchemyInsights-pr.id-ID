---
title: Masalah saat mengatur ulang kata sandi
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
ms.openlocfilehash: 535b5273d367e24ac45b3f60dbc7b6a2da6a3d9affa5a67499989d19a1904768
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039969"
---
# <a name="problems-resetting-password"></a>Masalah dalam mengatur ulang kata sandi

Berikut ini adalah beberapa masalah yang mungkin Anda hadapi ketika mereset kata sandi dan solusi yang memungkinkan:

**Saya mengalami masalah dengan pengaturan ulang kata sandi yang tidak dicakup dalam kategori lain**

- Pastikan Anda memiliki wewenang untuk mengatur ulang kata sandi. Hanya administrator global, kata sandi, dan pengguna yang bisa mereset kata sandi pengguna. Administrator global juga dapat mengatur ulang kata sandi administrator istimewa lainnya.
- Pastikan bahwa Anda memahami persyaratan lisensi:
    - Anda harus memiliki setidaknya satu lisensi yang ditetapkan di organisasi Anda
        - Pengguna awan saja - Semua Office 365 (O365) berbayar SKU, atau Azure AD Basic
        - Pengguna lokal dan/atau awan - Azure AD Premium P1 atau P2, Enterprise Mobility + Security (EMS), atau Secure Productive Enterprise (SPE)
        - Untuk membaca selengkapnya tentang persyaratan lisensi, lihat artikel [Persyaratan lisensi untuk pengaturan ulang kata sandi layanan mandiri Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)

**Saya mengalami masalah dalam menguji kebijakan atur ulang kata sandi yang saya atur**

- Kebijakan yang baru diterapkan bisa membutuhkan waktu beberapa menit untuk mereplikasi seluruh pusat data dan titik akhir. Jarak fisik dari pusat data juga akan memengaruhi seberapa cepat perubahan diterapkan.
- Uji dengan pengguna akhir, bukan administrator, dan uji coba dengan satu set pengguna kecil. Kebijakan yang dikonfigurasi di portal Azure HANYA berlaku bagi pengguna akhir, bukan administrator. Microsoft memberlakukan kebijakan pengaturan ulang kata sandi dua pintu default yang kuat untuk setiap peran administrator Azure (Contoh: Administrator Global, Administrator Staf Dukungan, Administrator Kata Sandi, dll.)
    - Pelajari selengkapnya tentang [kebijakan untuk administrator](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).

**Saya ingin menggunakan pengaturan ulang kata sandi tapi saya tidak ingin membuat pengguna saya mendaftarkan info keamanan tambahan**

Mengisi data untuk pengguna Anda terlebih dahulu sehingga mereka tidak perlu melakukannya! - Sebagai administrator Anda dapat mengatur properti telepon dan email untuk pengguna sebelum meluncurkan pengaturan ulang kata sandi ke organisasi. Anda dapat melakukan hal ini menggunakan API, PowerShell, atau Azure AD Koneksi. Informasi selengkapnya di sini:
- [Menyebarkan reset kata sandi tanpa mengharuskan pengguna untuk mendaftar](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Data apa yang digunakan oleh reset kata sandi](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Tombol reset kata sandi berwarna abu-abu**

Anda tidak diizinkan untuk mengatur ulang kata sandi pengguna ini. Hanya administrator global, kata sandi, dan pengguna yang bisa mereset kata sandi pengguna. Administrator global juga dapat mengatur ulang kata sandi administrator istimewa lainnya.

**Saya tidak melihat kata sandi mereset blade**

Anda tidak diizinkan untuk mengatur ulang kata sandi. Hanya administrator global, kata sandi, dan pengguna yang bisa mereset kata sandi pengguna. Administrator global juga dapat mengatur ulang kata sandi administrator istimewa lainnya.

**Saya tidak melihat blade integrasi di tempat dalam pengaturan ulang kata sandi**

- Blade integrasi di tempat hanya muncul di lingkungan hibrid - artinya Anda menggunakan kembali kata sandi untuk memanipulasi kata sandi pengguna lokal.
- Anda tidak melihat blade ini jika:
    - Anda tidak menggunakan kembali kata sandi
    - Ada masalah dengan penginstalan/konektivitas penulisan kata sandi
    - Ada masalah dengan instalasi/konektivitas Azure AD Koneksi
    - Untuk langkah pemecahan masalah selengkapnya terkait masalah dengan kembali menulis kata sandi, lihat bagian Memecahkan masalah [penulisan kembali kata sandi](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Saya tidak tahu cara mengatur ulang kata sandi pengguna**

1. Masuk ke portal Azure sebagai admin yang tepat.
1. Buka blade Pengguna dan grup, pilih **Semua Pengguna.**
1. Pilih pengguna dari daftar.
1. Untuk pengguna yang dipilih, pilih **Gambaran Umum**, lalu di bilah perintah, klik Reset **kata sandi.**
1. Ikuti instruksi di layar.
    - Hanya mereset yang dilakukan melalui portal Azure mendukung penulisan kembali kata sandi.

**Saya mereset kata sandi pengguna di tempat dari portal Office 365 Admin atau Office 365 seluler tapi pengguna masih tidak bisa masuk**

Password Writeback tidak didukung di portal ini. Mengatur ulang kata sandi pengguna lagi di portal Azure - portal.azure.com

