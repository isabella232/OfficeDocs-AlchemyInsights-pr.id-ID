---
title: Kesalahan aplikasi
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "7841"
ms.openlocfilehash: ce4c89da79112726ed4fb25527edc8d082bd37f239595b9eab7279abeeecfd7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931452"
---
# <a name="application-errors"></a>Kesalahan aplikasi

Mencari informasi tentang kode **kesalahan AADSTS** yang dikembalikan dari layanan token keamanan Azure Active Directory (Azure AD)? Baca [kode kesalahan otorisasi dan Autentikasi Azure AD](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) untuk menemukan deskripsi kesalahan AADSTS, perbaikan, dan beberapa solusi yang disarankan.

Kesalahan otorisasi dapat merupakan akibat dari beberapa masalah yang berbeda, yang sebagian besar menghasilkan kesalahan 401 atau 403. Misalnya, hal berikut ini dapat menyebabkan kesalahan otorisasi:

- Kesalahan [aliran akuisisi token akses](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- [Lingkup izin](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) dikonfigurasi dengan buruk 
- Kurangnya [persetujuan](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

Untuk mengatasi kesalahan otorisasi umum, cobalah langkah-langkah yang disediakan di bawah ini yang paling sesuai dengan kesalahan yang Anda terima. Mungkin lebih dari satu yang berlaku.

**Kesalahan tidak sah 401: Apakah token Anda valid?**

Pastikan bahwa aplikasi Anda menyajikan token akses yang valid ke Microsoft Graph sebagai bagian dari permintaan. Kesalahan ini sering kali berarti bahwa token akses mungkin hilang di header permintaan autentikasi HTTP atau token tidak valid atau telah kedaluwarsa. Kami sangat menyarankan agar Anda menggunakan Pustaka [Autentikasi Microsoft (MSAL, Microsoft Authentication Library) untuk](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) akuisisi token akses. Selain itu, kesalahan ini dapat terjadi jika Anda mencoba menggunakan token akses terdelegasi yang diberikan ke akun Microsoft pribadi untuk mengakses API yang hanya mendukung akun kerja atau sekolah (akun organisasi).

**Kesalahan terlarang 403: Sudahkah Anda memilih set izin yang tepat?**

Periksa apakah Anda telah meminta serangkaian izin yang benar berdasarkan API Microsoft Graph pada panggilan aplikasi Anda. Izin paling sedikit hak istimewa yang direkomendasikan disediakan di semua topik metode referensi API Graph Microsoft. Selain itu, izin tersebut harus diberikan pada aplikasi oleh pengguna atau administrator. Memberikan izin yang biasanya terjadi melalui halaman persetujuan atau dengan memberikan izin menggunakan blade registrasi aplikasi Portal Azure. Dari blade **Pengaturan** untuk aplikasi tersebut, klik **Izin yang Diperlukan**, lalu klik **Berikan Izin**.

- [Izin Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Memahami izin dan persetujuan Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**Kesalahan terlarang 403: Apakah aplikasi Anda mendapatkan token untuk mencocokkan izin yang dipilih?**

Pastikan bahwa tipe izin yang diminta atau diberikan sesuai dengan tipe token akses yang diperoleh aplikasi Anda. Anda mungkin meminta dan memberikan izin aplikasi, tetapi menggunakan token alur kode interaktif yang didelegasikan, bukan token aliran kredensial klien, atau meminta dan memberikan izin yang didelegasikan, tetapi menggunakan token alur kredensial klien, bukan token aliran kode yang didelegasikan.

- [Dapatkan akses atas nama pengguna dan izin yang didelegasikan](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v2.0 - alur kode otorisasi OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Dapatkan akses tanpa pengguna (layanan daemon) dan izin aplikasi](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v2.0 - alur kredensial klien OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**Kesalahan terlarang 403: Mengatur ulang kata sandi**

Saat ini, tidak ada izin layanan-ke-layanan daemon izin aplikasi yang mengizinkan pengaturan ulang kata sandi pengguna. API ini hanya didukung menggunakan alur kode interaktif yang didelegasikan dengan administrator yang masuk.

- [Izin Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference)

**Terlarang 403: Apakah pengguna memiliki akses dan apakah dilisensikan?**

Untuk aliran kode yang didelegasikan, Microsoft Graph akan mengevaluasi jika permintaan diizinkan berdasarkan izin yang diberikan kepada aplikasi dan izin yang diberikan oleh pengguna yang masuk. Secara umum, kesalahan ini menunjukkan bahwa pengguna tidak memiliki hak istimewa untuk melakukan permintaan atau pengguna tidak dilisensikan untuk data yang diakses. Hanya pengguna dengan izin atau lisensi yang diperlukan yang dapat membuat permintaan berhasil.

**Terlarang 403: Apakah Anda memilih API sumber daya yang benar?**

Layanan API seperti Microsoft Graph memeriksa bahwa klaim (audiens) aud di token akses yang diterima sesuai dengan nilai yang diharapkan untuk dirinya sendiri, dan jika tidak, itu mengakibatkan kesalahan Dilarang 403. Kesalahan umum yang mengakibatkan kesalahan ini adalah mencoba menggunakan token yang diperoleh untuk API Grafik Azure AD, API Outlook, atau API SharePoint/OneDrive untuk menghubungi Microsoft Graph (atau sebaliknya). Pastikan sumber daya (atau lingkup) yang aplikasi Anda memperoleh token cocok dengan API yang dihubungi aplikasi.

**Permintaan Buruk 400 atau Terlarang 403: Apakah pengguna mematuhi kebijakan akses bersyarat (CA) organisasinya?**

Berdasarkan kebijakan CA organisasi, pengguna yang mengakses sumber daya Microsoft Graph melalui aplikasi Anda mungkin ditandingi untuk informasi tambahan yang tidak ada di token akses yang didapatkan oleh aplikasi Anda pada awalnya. Dalam kasus ini, aplikasi Anda menerima 400 dengan kesalahan *interaction_required* selama proses akuisisi token akses atau 403 dengan kesalahan *insufficient_claims* ketika menghubungi Microsoft Graph. Dalam kedua kasus tersebut, respons kesalahan berisi informasi tambahan yang dapat diberikan ke titik akhir otorisasi untuk tantangan pengguna terhadap informasi tambahan (seperti multi-factor authentication atau pendaftaran perangkat).

- [Menangani tantangan akses bersyarat menggunakan MSAL ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Panduan pengembang untuk akses bersyarat Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
