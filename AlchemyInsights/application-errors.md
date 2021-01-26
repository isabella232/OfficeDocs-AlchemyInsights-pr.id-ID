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
ms.openlocfilehash: 2ef90b54ce222a06740e05891fabe87b6565cb14
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/25/2021
ms.locfileid: "49984587"
---
# <a name="application-errors"></a>Kesalahan aplikasi

Mencari informasi tentang **kode kesalahan Aadsts** yang dikembalikan dari layanan token keamanan (STS) Azure Active Directory (Azure AD)? Baca [kode kesalahan autentikasi dan autentikasi AZURE AD](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) untuk menemukan deskripsi kesalahan, perbaikan, dan beberapa solusi yang disarankan.

Kesalahan otorisasi dapat berupa beberapa masalah yang berbeda, yang sebagian besar menghasilkan kesalahan 401 atau 403. Misalnya, Semua hal berikut ini dapat menyebabkan kesalahan otorisasi:

- [Aliran akuisisi token akses](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) tidak benar 
- [Lingkup izin](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) yang dikonfigurasi dengan buruk 
- Kurangnya [persetujuan](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

Untuk mengatasi kesalahan otorisasi umum, coba langkah yang disediakan di bawah ini yang paling cocok dengan kesalahan yang Anda terima. Lebih dari satu mungkin berlaku.

**kesalahan tidak sah 401: Apakah token Anda valid?**

Pastikan bahwa aplikasi Anda menyajikan token akses yang valid ke Microsoft graph sebagai bagian dari permintaan. Kesalahan ini sering kali berarti token Access mungkin tidak ditemukan dalam header permintaan autentikasi HTTP atau token tidak valid atau telah kedaluwarsa. Kami sangat menyarankan agar Anda menggunakan [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) untuk akuisisi token Access. Selain itu, kesalahan ini dapat terjadi jika Anda mencoba menggunakan token akses delegasi yang diberikan ke akun Microsoft pribadi untuk mengakses API yang hanya mendukung akun kerja atau sekolah (akun organisasi).

**kesalahan Forbidden 403: Apakah Anda telah memilih kumpulan izin yang tepat?**

Pastikan bahwa Anda telah meminta kumpulan izin yang benar berdasarkan Microsoft graph melakukan panggilan aplikasi Anda. Izin paling tidak istimewa yang direkomendasikan disediakan dalam semua topik metode referensi API Microsoft graph. Selain itu, izin tersebut harus diberikan kepada aplikasi oleh pengguna atau administrator. Pemberian izin biasanya terjadi melalui halaman persetujuan atau dengan memberi izin menggunakan pisau registrasi aplikasi Azure portal. Dari bilah **pengaturan** untuk aplikasi, klik izin yang **diperlukan**, lalu klik **Berikan izin**.

- [Izin Microsoft graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Memahami izin dan izin Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**kesalahan Forbidden 403: Apakah aplikasi Anda mendapatkan token untuk mencocokkan izin yang dipilih?**

Pastikan bahwa tipe izin yang diminta atau diberikan cocok dengan tipe token Access yang diakuisisi aplikasi Anda. Anda mungkin meminta dan memberikan izin aplikasi tapi menggunakan aliran kode interaktif terdelegasi bukan token aliran kredensial klien, atau meminta dan memberikan izin yang didelegasikan tetapi menggunakan token aliran kredensial klien dan bukan token alur aliran kode.

- [Mendapatkan akses atas nama pengguna dan izin yang didelegasikan](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v 2.0-alur kode otorisasi OAuth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Dapatkan akses tanpa pengguna (layanan daemon) dan izin aplikasi](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v 2.0-aliran kredensial klien 2,0 OAuth](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**kesalahan terlarang 403: mereset kata sandi**

Saat ini, tidak ada izin layanan daemon izin aplikasi ke layanan yang memperbolehkan mereset kata sandi pengguna. Api ini hanya didukung menggunakan alur kode delegasi interaktif dengan administrator masuk.

- [Izin Microsoft graph](https://docs.microsoft.com/graph/permissions-reference)

**403 dilarang: Apakah pengguna memiliki akses dan apakah mereka memiliki lisensi?**

Untuk alur kode terdelegasi, Microsoft graph mengevaluasi jika permintaan diperbolehkan berdasarkan izin yang diberikan kepada aplikasi dan izin yang dimiliki pengguna yang masuk. Secara umum, kesalahan ini menunjukkan bahwa pengguna tidak cukup istimewa untuk melakukan permintaan atau pengguna tidak dilisensikan untuk data yang sedang diakses. Hanya pengguna dengan izin atau lisensi yang diperlukan yang dapat membuat permintaan berhasil.

**403 dilarang: Apakah Anda memilih API sumber daya yang benar?**

Layanan API seperti Microsoft graph memeriksa apakah klaim AUD (audiens) dalam token akses yang diterima sesuai dengan nilai yang diharapkan, dan jika tidak, maka akan menghasilkan kesalahan 403 Forbidden. Kesalahan umum yang mengakibatkan kesalahan ini mencoba menggunakan token yang diperoleh untuk api Azure AD graph, api Outlook, atau SharePoint/OneDrive api untuk memanggil Microsoft graph (atau sebaliknya). Pastikan bahwa sumber daya (atau lingkup) yang diperoleh aplikasi Anda untuk mendapatkan token sesuai dengan API yang sedang dihubungi aplikasi.

**400 Bad request atau 403 Forbidden: Apakah pengguna mematuhi kebijakan conditional Access (CA) organisasi mereka?**

Berdasarkan kebijakan CA organisasi, pengguna yang mengakses sumber daya Microsoft graph melalui aplikasi Anda mungkin ditantang untuk informasi tambahan yang tidak ada dalam token Access yang diperoleh aplikasi Anda. Dalam kasus ini, aplikasi Anda menerima 400 dengan kesalahan *interaction_required* selama akuisisi token access atau 403 dengan kesalahan *Insufficient_claims* saat memanggil Microsoft graph. Dalam kedua kasus, respons kesalahan berisi informasi tambahan yang dapat disajikan ke titik akhir otorisasi untuk menantang pengguna untuk informasi tambahan (seperti autentikasi multi-faktor atau pendaftaran perangkat).

- [Menangani tantangan akses bersyarat menggunakan MSAL ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Panduan pengembang untuk akses bersyarat Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
