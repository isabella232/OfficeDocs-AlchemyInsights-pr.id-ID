---
title: Masalah API Graph Microsoft
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
- "9004345"
- "7759"
ms.openlocfilehash: 9df021211c8a65997889d9303dbf28a27104cfa95841d4cb810427c652ba0784
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975896"
---
# <a name="microsoft-graph-api-issues"></a>Masalah API Graph Microsoft

Topik ini mungkin juga berlaku untuk pengembang yang masih menggunakan API Azure AD Graph. Namun, sangat **dianjurkan agar** Anda menggunakan Microsoft Graph semua skenario manajemen direktori, identitas, dan akses.

**Masalah autentikasi atau otorisasi**

- Jika aplikasi Anda tidak dapat memperoleh **token** untuk menghubungi Microsoft Graph, pilih Masalah dengan mendapatkan token akses **(Autentikasi)** kategori Microsoft Graph untuk mendapatkan bantuan dan dukungan yang lebih spesifik tentang topik ini.
- Jika aplikasi Anda menerima **401 atau 403** kesalahan otorisasi saat menghubungi Microsoft Graph, pilih kategori Mendapatkan akses yang ditolak **(Otorisasi)** API Microsoft Graph untuk mendapatkan bantuan dan dukungan yang lebih spesifik tentang topik ini.

**Saya ingin menggunakan Microsoft Graph, tetapi tidak yakin harus memulai dari mana**

- [Gambaran umum Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Gambaran umum tentang Identitas dan Manajemen Akses di Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Mulai membangun aplikasi Microsoft Graph baru](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** - Uji Graph API Microsoft di penyewa Anda atau penyewa demo

**Saya ingin menggunakan Microsoft Graph, tapi apakah aplikasi ini mendukung API direktori v1.0 yang saya perlukan?**

Microsoft Graph adalah API yang disarankan untuk manajemen direktori, identitas, dan akses. Namun, masih ada beberapa jarak antara apa yang mungkin dilakukan di Azure AD Graph dan Microsoft Graph. Tinjau artikel berikut, yang menyoroti perbedaan yang paling baru untuk membantu dalam pilihan Anda:

- [Perbedaan tipe sumber daya antara Azure AD Graph dan Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Perbedaan properti antara Azure AD Graph dan Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Perbedaan metode antara Azure AD dan Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**API yang saya panggil tidak berfungsi - di mana saya bisa melakukan lebih banyak pengujian?**

**Microsoft Graph Explorer** - Uji api Graph Microsoft dalam penyewa atau penyewa demo dan lihat juga contoh **kueri** di Microsoft Graph Explorer.

**Aplikasi saya terlalu lambat dan juga tidak dapat digunakan. Penyempurnaan apa yang dapat saya buat?**

Bergantung pada skenario Anda, ada berbagai opsi menurut Anda untuk membuat aplikasi Anda lebih berkinerja, dan dalam beberapa kasus, lebih sedikit rentan terhadap layanan (ketika Anda melakukan terlalu banyak panggilan).

- [Praktik Graph terbaik Microsoft](https://docs.microsoft.com/graph/best-practices-concept)
- [Permintaan kumpulan](https://docs.microsoft.com/graph/json-batching)
- [Lacak perubahan melalui kueri delta](https://docs.microsoft.com/graph/delta-query-overview)
- [Mendapatkan pemberitahuan tentang perubahan melalui webhooks](https://docs.microsoft.com/graph/webhooks)
- [Panduan pembatasan](https://docs.microsoft.com/graph/throttling)

**Di mana saya bisa menemukan informasi selengkapnya tentang kesalahan dan masalah yang diketahui?**

- [Informasi Graph respons kesalahan Microsoft](https://docs.microsoft.com/graph/errors)
- [Masalah umum dengan Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Di mana saya dapat memeriksa status ketersediaan dan konektivitas layanan?**

Ketersediaan dan konektivitas layanan dasar yang dapat diakses melalui Microsoft Graph dapat berdampak pada ketersediaan dan kinerja Microsoft Graph.

- Untuk Azure Active Directory kesehatan layanan, periksa status layanan **Keamanan + Identitas** yang tercantum di halaman status [Azure.](https://azure.microsoft.com/status/)
- Untuk Office yang berkontribusi pada Microsoft Graph, periksa status layanan yang tercantum [di Office Service Health Dashboard.](https://portal.office.com/adminportal/home#/servicehealth)

Kesalahan otorisasi Graph Microsoft bisa diakibatkan dari beberapa masalah berbeda, yang sebagian besar mengakibatkan kesalahan 401 atau 403. Misalnya, hal berikut ini dapat menyebabkan kesalahan otorisasi:

- Kesalahan [aliran akuisisi token akses](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- [Lingkup izin](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) dikonfigurasi dengan buruk
- Kurangnya [persetujuan](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

***Akhir dukungan untuk Azure Active Directory Authentication Library (ADAL) dan API Azure AD Graph (AAD Graph)***

**Mulai 30 Juni 2020,** kami tidak akan lagi menambahkan fitur baru untuk ADAL dan Azure AD Graph. Kami akan terus menyediakan dukungan teknis dan pembaruan keamanan, namun tidak akan lagi menyediakan pembaruan fitur.

**Mulai 30 Juni 2022,** kami akan mengakhiri dukungan untuk ADAL dan Azure AD Graph dan tidak akan lagi menyediakan dukungan teknis atau pembaruan keamanan.

Aplikasi yang menggunakan ADAL di versi OS yang sudah ada akan terus berfungsi setelah saat ini, tetapi tidak akan *mendapatkan dukungan teknis atau pembaruan keamanan.*

Aplikasi yang menggunakan Azure AD Graph setelah waktu ini mungkin tidak lagi menerima respons dari titik akhir Azure AD Graph akhir.

**Migrasi ADAL**

Kami merekomendasikan Anda memperbarui ke [Pustaka Autentikasi Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), yang memiliki fitur dan pembaruan keamanan terbaru.

Jika Anda menggunakan aplikasi Microsoft, ketahui bahwa Microsoft sedang dalam proses migrasi aplikasinya ke MSAL hingga tenggat waktu akhir dukungan, yang memastikan mereka akan mendapatkan manfaat dari penyempurnaan fitur dan keamanan MSAL yang sedang berlangsung.

1. [Baca FAQ ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Pelajari tentang cara melakukan migrasi aplikasi pada basis per platform](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Jika memerlukan bantuan memahami aplikasi mana yang menggunakan ADAL, kami menyarankan Anda meninjau semua kode sumber aplikasi, dan jika ada, hubungi ISVs atau penyedia aplikasi. Dukungan Microsoft juga dapat menyediakan daftar semua aplikasi non-Microsoft ADAL di penyewa Anda.

**Migrasi Grafik AAD**

Untuk aplikasi yang menggunakan Azure AD Graph, ikuti panduan kami untuk melakukan migrasi aplikasi [Azure AD Graph ke Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).

1. [Daftar periksa migrasi kami menyediakan poin memulai](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. Portal pendaftaran aplikasi Azure Anda memperlihatkan aplikasi mana yang menggunakan Grafik AAD. Kami menyarankan Anda meninjau semua kode sumber aplikasi, dan jika memungkinkan, hubungi semua ISV atau penyedia aplikasi. Dukungan Microsoft juga dapat menyediakan daftar semua penggunaan AAD Graph penyewa Anda.
3. Agar aplikasi Anda mengakses data di Microsoft Graph, pengguna atau administrator harus memberikan izin yang tepat melalui proses persetujuan. Referensi [izin Graph Microsoft](https://docs.microsoft.com/graph/permissions-reference) mencantumkan izin yang terkait dengan setiap rangkaian utama API Microsoft Graph. Panduan juga tentang cara menggunakan izin.
