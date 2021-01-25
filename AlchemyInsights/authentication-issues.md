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
ms.openlocfilehash: 53bd0d8f8edaead519d0282239d3a6d338b297b9
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974486"
---
# <a name="authentication-issues"></a>Masalah autentikasi

**Mencari informasi tentang kode kesalahan AADSTS yang dikembalikan dari layanan token keamanan (STS) Azure Active Directory (Azure AD)?** Lihat [kode kesalahan autentikasi dan autentikasi AZURE AD](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) untuk menemukan deskripsi kesalahan, perbaikan, dan beberapa solusi yang disarankan.

Kesalahan otorisasi dapat berupa beberapa masalah yang berbeda, yang sebagian besar menghasilkan kesalahan 401 atau 403. Misalnya, masalah berikut ini bisa menyebabkan kesalahan otorisasi:

- [Aliran akuisisi token akses](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) tidak benar 
- [Lingkup izin](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) yang dikonfigurasi dengan buruk 
- Kurangnya [persetujuan](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)

Untuk mengatasi kesalahan otorisasi umum, coba langkah yang diberikan di bawah ini yang paling cocok dengan kesalahan yang Anda terima. Lebih dari satu langkah mungkin berlaku untuk kesalahan yang Anda terima.

- **kesalahan tidak sah 401: Apakah token Anda valid?**

Pastikan bahwa aplikasi Anda menyajikan token akses yang valid ke Microsoft graph sebagai bagian dari permintaan. Kesalahan ini sering kali berarti token Access mungkin tidak ditemukan dalam header permintaan autentikasi HTTP atau token tidak valid atau telah kedaluwarsa. Kami sangat menyarankan agar Anda menggunakan Microsoft Authentication Library (MSAL) untuk akuisisi token Access. Selain itu, kesalahan ini dapat terjadi jika Anda mencoba menggunakan token akses delegasi yang diberikan ke akun Microsoft pribadi untuk mengakses API yang hanya mendukung akun kerja atau sekolah (akun organisasi).

**kesalahan Forbidden 403: Apakah Anda telah memilih kumpulan izin yang tepat?**

Pastikan bahwa Anda telah meminta kumpulan izin yang benar berdasarkan Microsoft graph melakukan panggilan aplikasi Anda. Izin paling tidak-istimewa yang direkomendasikan disediakan dalam semua topik metode referensi API Microsoft graph. Selain itu, izin tersebut harus diberikan kepada aplikasi oleh pengguna atau administrator. Pemberian izin biasanya terjadi melalui halaman persetujuan atau penggunaan Blade registrasi aplikasi Azure portal. Dari bilah **pengaturan** untuk aplikasi, klik izin yang **diperlukan**, lalu klik **Berikan izin**. Untuk informasi selengkapnya, lihat:

- [Izin Microsoft graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Memahami izin dan izin Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**kesalahan Forbidden 403: Apakah aplikasi Anda mendapatkan token untuk mencocokkan izin yang dipilih?**

Pastikan bahwa tipe izin yang diminta atau diberikan sesuai dengan tipe token Access yang diperoleh aplikasi Anda. Anda mungkin meminta dan memberikan izin aplikasi tapi menggunakan aliran kode interaktif terdelegasi bukan token aliran kredensial klien, atau meminta dan memberikan izin yang didelegasikan tetapi menggunakan token aliran kredensial klien dan bukan token aliran kode terdelegasi.

Untuk informasi selengkapnya yang terkait dengan perolehan token, lihat:

- [Mendapatkan akses atas nama pengguna dan izin yang didelegasikan](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v 2.0-alur kode otorisasi OAuth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Dapatkan akses tanpa pengguna (layanan daemon) dan izin aplikasi](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v 2.0-aliran kredensial klien 2,0 OAuth](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**kesalahan terlarang 403: mereset kata sandi**

Saat ini, tidak ada izin layanan daemon izin aplikasi ke layanan yang memperbolehkan mereset kata sandi pengguna. Api ini hanya didukung menggunakan alur kode delegasi interaktif dengan administrator masuk. Untuk informasi selengkapnya, lihat [izin Microsoft graph](https://docs.microsoft.com/graph/permissions-reference).

**403 dilarang: Apakah pengguna memiliki akses dan apakah mereka memiliki lisensi?**

Untuk alur kode terdelegasi, Microsoft graph mengevaluasi apakah permintaan telah diizinkan berdasarkan izin yang diberikan kepada aplikasi dan izin yang dimiliki pengguna yang masuk. Secara umum, kesalahan ini menunjukkan bahwa pengguna tidak cukup istimewa untuk melakukan permintaan **atau** pengguna tidak dilisensikan untuk data yang sedang diakses. Hanya pengguna dengan izin atau lisensi yang diperlukan yang dapat membuat permintaan berhasil.

**403 dilarang: Apakah Anda memilih API sumber daya yang benar?**

Layanan API seperti Microsoft graph memeriksa bahwa klaim *AUD* (audiens) dalam token akses diterima sesuai dengan nilai yang diharapkan untuk dirinya sendiri, dan jika tidak, terjadi kesalahan 403 Forbidden. Kesalahan umum yang mengakibatkan kesalahan ini mencoba menggunakan token yang diperoleh untuk api Azure AD graph, api Outlook, atau SharePoint/OneDrive api untuk memanggil Microsoft graph (atau sebaliknya). Pastikan bahwa sumber daya (atau lingkup) yang diperoleh aplikasi Anda untuk mendapatkan token sesuai dengan API yang sedang dihubungi aplikasi.

**400 Bad request atau 403 Forbidden: Apakah pengguna mematuhi kebijakan conditional Access (CA) organisasi mereka?**

Berdasarkan kebijakan akses bersyarat (CA) organisasi, pengguna yang mengakses sumber daya Microsoft graph melalui aplikasi Anda mungkin ditantang untuk informasi tambahan yang tidak ada dalam token Access yang diperoleh aplikasi Anda. Dalam kasus ini, aplikasi Anda menerima **400 dengan kesalahan *interaction_required*** selama akuisisi token Access atau **403 dengan kesalahan *insufficient_claims*** saat memanggil Microsoft graph. Dalam kedua kasus, respons kesalahan berisi informasi tambahan yang dapat disajikan ke titik akhir resmi untuk menantang pengguna untuk informasi tambahan (seperti autentikasi multi-faktor atau pendaftaran perangkat).

Untuk informasi lebih lanjut terkait dengan akses bersyarat, lihat:

- [Menangani tantangan akses bersyarat menggunakan MSAL](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Panduan pengembang untuk akses bersyarat Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

**_Akhir dukungan untuk Azure Active Directory Authentication Library (ADAL) dan AZURE AD GRAPH api (GRAF AAD)_* _

- Mulai tanggal 30 Juni 2020, kami tidak akan lagi menambahkan fitur baru ke pustaka autentikasi direktori aktif Azure (ADAL) dan Azure AD graph API (Graf AAD). Kami akan terus menyediakan dukungan teknis dan pembaruan keamanan tetapi tidak lagi menyediakan pembaruan fitur.
- Mulai 30 Juni 2022, kami akan mengakhiri dukungan untuk Graf ADAL dan AAD dan tidak lagi menyediakan dukungan teknis atau pembaruan keamanan.
    - Aplikasi yang menggunakan ADAL pada versi OS yang sudah ada akan terus berfungsi setelah waktu ini tetapi tidak akan mendapatkan dukungan teknis atau pembaruan keamanan apa pun.
    - Aplikasi menggunakan grafik AAD setelah waktu ini mungkin tidak lagi menerima respons dari titik akhir Graf AAD.

_ *Migrasi ADAL**

Sebaiknya Perbarui ke [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), yang memiliki fitur dan pembaruan keamanan terbaru. Rekomendasi ini dalam konteks Microsoft melakukan migrasi aplikasinya ke MSAL pada batas akhir dukungan. Tujuan migrasi Microsoft Apps ke MSAL adalah memastikan bahwa aplikasi tersebut mendapatkan manfaat dari penyempurnaan fitur dan keamanan yang sedang berlangsung.

- [Membaca FAQ ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Pelajari tentang cara melakukan migrasi aplikasi secara per platform](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Jika Anda memerlukan bantuan untuk memahami aplikasi mana yang menggunakan ADAL, kami menyarankan agar Anda meninjau semua kode sumber aplikasi Anda, dan jika ada, hubungi vendor perangkat lunak independen (ISVs) atau penyedia aplikasi lainnya. Dukungan Microsoft juga bisa memberi Anda daftar semua aplikasi non-Microsoft ADAL di penyewa Anda.

**Migrasi Graf AAD**

Untuk aplikasi yang menggunakan grafik AAD, ikuti panduan kami untuk melakukan [migrasi aplikasi AZURE AD graph ke Microsoft graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [Daftar Periksa migrasi kami menyediakan titik mulai](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- Portal pendaftaran aplikasi Azure memperlihatkan aplikasi mana yang menggunakan grafik AAD. Kami menyarankan agar Anda meninjau semua kode sumber aplikasi, dan jika ada, hubungi penyedia ISVs atau aplikasi apa pun. Dukungan Microsoft juga bisa memberi Anda informasi tentang semua penggunaan grafik AAD dalam penyewa Anda.

 










