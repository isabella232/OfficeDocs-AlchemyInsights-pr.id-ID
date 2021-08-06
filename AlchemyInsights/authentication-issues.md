---
title: Masalah autentikasi
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7748"
- "9004339"
ms.openlocfilehash: c7e6d96940f8d7052ee4b49b22c0d1d7d5bd5f9277f4a7eff709def1da2e13af
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019511"
---
# <a name="authentication-issues"></a>Masalah autentikasi

**Mencari informasi tentang kode kesalahan AADSTS yang dikembalikan dari layanan token keamanan (STS) Azure Active Directory (Azure AD)?** Lihat [kode kesalahan Otorisasi dan Autentikasi Azure AD](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) untuk menemukan deskripsi kesalahan AADSTS, perbaikan, dan beberapa solusi yang disarankan.

Kesalahan otorisasi dapat merupakan akibat dari beberapa masalah yang berbeda, yang sebagian besar menghasilkan kesalahan 401 atau 403. Misalnya, masalah berikut ini semua dapat mengakibatkan kesalahan otorisasi:

- Kesalahan [aliran akuisisi token akses](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) 
- [Lingkup izin](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) dikonfigurasi dengan buruk 
- Kurangnya [persetujuan](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)

Untuk mengatasi kesalahan otorisasi umum, cobalah langkah-langkah yang disediakan di bawah ini yang paling sesuai dengan kesalahan yang Anda terima. Lebih dari satu langkah dapat diterapkan untuk kesalahan yang Anda terima.

**Kesalahan tidak sah 401: Apakah token Anda valid?**

Pastikan bahwa aplikasi Anda menyajikan token akses valid ke Microsoft Graph sebagai bagian dari permintaan. Kesalahan ini sering kali berarti bahwa token akses mungkin hilang di header permintaan autentikasi HTTP atau token tidak valid atau telah kedaluwarsa. Kami sangat menyarankan agar Anda menggunakan Pustaka Autentikasi Microsoft (MSAL) untuk akuisisi token akses. Selain itu, kesalahan ini dapat terjadi jika Anda mencoba menggunakan token akses terdelegasi yang diberikan ke akun Microsoft pribadi untuk mengakses API yang hanya mendukung akun kerja atau sekolah (akun organisasi).

**Kesalahan terlarang 403: Sudahkah Anda memilih set izin yang tepat?**

Pastikan bahwa Anda telah meminta set izin yang benar berdasarkan API Microsoft Graph untuk panggilan aplikasi. Izin paling tidak istimewa yang disarankan disediakan di semua topik metode referensi API Microsoft Graph. Selain itu, izin tersebut harus diberikan pada aplikasi oleh pengguna atau administrator. Memberikan izin biasanya terjadi melalui halaman persetujuan atau penggunaan blade pendaftaran aplikasi Azure Portal. Dari blade **Pengaturan** untuk aplikasi tersebut, klik **Izin yang Diperlukan**, lalu klik **Berikan Izin**. Untuk informasi selengkapnya, lihat:

- [Izin Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Memahami izin dan persetujuan Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**Kesalahan terlarang 403: Apakah aplikasi Anda mendapatkan token untuk mencocokkan izin yang dipilih?**

Pastikan bahwa tipe izin yang diminta atau diberikan sesuai dengan tipe token akses yang diperoleh aplikasi Anda. Anda mungkin meminta dan memberikan izin aplikasi, tetapi menggunakan token alur kode interaktif yang didelegasikan, bukan token alur kredensial klien, atau meminta dan memberikan izin delegasi tetapi menggunakan token alur kredensial klien, bukan token alur kode yang didelegasikan.

Untuk informasi selengkapnya terkait memperoleh token, lihat:

- [Dapatkan akses atas nama pengguna dan izin yang didelegasikan](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v2.0 - alur kode otorisasi OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Dapatkan akses tanpa pengguna (layanan daemon) dan izin aplikasi](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v2.0 - alur kredensial klien OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**Kesalahan terlarang 403: Mengatur ulang kata sandi**

Saat ini, tidak ada izin layanan-ke-layanan daemon izin aplikasi yang mengizinkan pengaturan ulang kata sandi pengguna. API ini hanya didukung menggunakan alur kode interaktif yang didelegasikan dengan administrator yang masuk. Untuk informasi selengkapnya, lihat [izin Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference).

**Terlarang 403: Apakah pengguna memiliki akses dan apakah dilisensikan?**

Untuk alur kode yang didelegasikan, Microsoft Graph mengevaluasi apakah permintaan telah diizinkan berdasarkan izin yang diberikan ke aplikasi dan izin yang dimiliki pengguna yang masuk. Secara umum, kesalahan ini menunjukkan bahwa pengguna tidak memiliki hak istimewa untuk melakukan permintaan **atau** pengguna tidak dilisensikan untuk data yang diakses. Hanya pengguna dengan izin atau lisensi yang diperlukan yang dapat membuat permintaan berhasil.

**Terlarang 403: Apakah Anda memilih API sumber daya yang benar?**

Layanan API seperti Microsoft Graph memeriksa klaim *aud* (audiens) di token akses yang diterima cocok dengan nilai yang diharapkannya, dan jika tidak, Kesalahan terlarang 403 terjadi. Kesalahan umum yang mengakibatkan kesalahan ini adalah mencoba menggunakan token yang diperoleh untuk API Grafik Azure AD, API Outlook, atau API SharePoint/OneDrive untuk menghubungi Microsoft Graph (atau sebaliknya). Pastikan sumber daya (atau lingkup) yang aplikasi Anda memperoleh token cocok dengan API yang dihubungi aplikasi.

**Permintaan Buruk 400 atau Terlarang 403: Apakah pengguna mematuhi kebijakan akses bersyarat (CA) organisasinya?**

Berdasarkan kebijakan akses bersyarat (CA) organisasi, pengguna yang mengakses sumber daya Microsoft Graph melalui aplikasi Anda mungkin akan diminta informasi tambahan yang tidak ada dalam token akses yang awalnya diperoleh aplikasi Anda. Dalam kasus ini, aplikasi Anda menerima **400 dengan kesalahan *interaction_required*** selama proses akuisisi token akses atau **403 dengan kesalahan *insufficient_claims*** ketika menghubungi Microsoft Graph. Dalam kedua kasus, respons kesalahan berisi informasi tambahan yang dapat diberikan pada titik akhir yang sah untuk meminta pengguna informasi tambahan (seperti autentikasi multifaktor atau pendaftaran perangkat).

Untuk informasi selengkapnya yang terkait dengan akses bersyarat, lihat:

- [Menangani tantangan akses bersyarat menggunakan MSAL](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Panduan pengembang untuk akses bersyarat Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

***Akhir dukungan untuk Azure Active Directory Authentication Library (ADAL) dan API Azure AD Graph (AAD Graph)***

- Mulai tanggal 30 Juni 2020, kami tidak akan lagi menambahkan fitur baru ke Pustaka Autentikasi Azure Active Directory (ADAL) dan API Grafik Azure AD (Grafik AAD). Kami akan terus menyediakan dukungan teknis dan pembaruan keamanan, namun tidak akan lagi menyediakan pembaruan fitur.
- Mulai tanggal 30 Juni 2022, kami akan mengakhiri dukungan untuk ADAL dan Grafik AAD dan tidak akan lagi menyediakan dukungan teknis atau pembaruan keamanan.
    - Aplikasi yang menggunakan ADAL di versi OS yang sudah ada akan terus berfungsi setelah waktu ini, tetapi tidak akan mendapatkan dukungan teknis atau pembaruan keamanan apa pun.
    - Aplikasi yang menggunakan Grafik AAD setelah waktu ini mungkin tidak lagi menerima respons dari titik akhir Grafik AAD.

**Migrasi ADAL**

Kami merekomendasikan Anda memperbarui ke [Pustaka Autentikasi Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), yang memiliki fitur dan pembaruan keamanan terbaru. Rekomendasi ini sesuai dengan konteks Microsoft yang melakukan migrasi aplikasinya ke MSAL pada tenggat waktu akhir dukungan. Tujuan migrasi aplikasi Microsoft ke MSAL adalah untuk memastikan bahwa aplikasi mendapatkan manfaat dari penyempurnaan fitur dan keamanan MSAL yang sedang berlangsung.

- [Baca FAQ ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Pelajari tentang cara melakukan migrasi aplikasi pada basis per platform](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Jika memerlukan bantuan untuk memahami aplikasi mana yang menggunakan ADAL, kami menyarankan Anda meninjau semua kode sumber aplikasi, dan jika memungkinkan, hubungi vendor perangkat lunak independen (ISVs) atau penyedia aplikasi. Dukungan Microsoft juga dapat menyediakan daftar semua aplikasi non-Microsoft ADAL di penyewa Anda.

**Migrasi Grafik AAD**

Untuk aplikasi yang menggunakan Grafik AAD, ikuti panduan kami untuk [melakukan migrasi aplikasi Grafik Azure AD ke Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [Daftar periksa migrasi kami menyediakan poin memulai](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- Portal pendaftaran aplikasi Azure Anda memperlihatkan aplikasi mana yang menggunakan Grafik AAD. Kami menyarankan Anda meninjau semua kode sumber aplikasi, dan jika memungkinkan, hubungi semua ISV atau penyedia aplikasi. Dukungan Microsoft juga dapat menyediakan informasi semua penggunaan Grafik AAD di penyewa Anda.

 










