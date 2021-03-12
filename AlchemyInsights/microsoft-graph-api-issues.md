---
title: Masalah API Microsoft graph
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
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/29/2021
ms.locfileid: "50714151"
---
# <a name="microsoft-graph-api-issues"></a>Masalah API Microsoft graph

Topik ini juga mungkin berlaku untuk pengembang masih menggunakan Azure AD graph API. Namun, **sangat disarankan agar** Anda menggunakan Microsoft graph untuk semua skenario manajemen direktori, identitas, dan akses Anda.

**Masalah autentikasi atau otorisasi**

- Jika aplikasi Anda **tidak dapat memperoleh token** untuk menghubungi Microsoft graph, pilih **masalah dengan mendapatkan kategori token Access (autentikasi)** Microsoft graph untuk mendapatkan bantuan dan dukungan yang lebih spesifik tentang topik ini.
- Jika aplikasi Anda **menerima kesalahan otorisasi 401 atau 403** saat memanggil Microsoft graph, pilih kategori Dapatkan Microsoft graph **error (otorisasi) Access ditolak (Authorization)** untuk mendapatkan bantuan dan dukungan yang lebih spesifik tentang topik ini.

**Saya ingin menggunakan Microsoft graph, tapi tidak yakin di mana memulai**

- [Gambaran Umum Microsoft graph](https://docs.microsoft.com/graph/overview)
- [Gambaran umum manajemen identitas dan akses di Microsoft graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Membuat aplikasi Microsoft graph yang mulai](https://docs.microsoft.com/graph/)
- **Microsoft graph Explorer** -uji Microsoft graph api dalam penyewa atau penyewa demo Anda

**Saya ingin menggunakan Microsoft graph, tetapi apakah aplikasi ini mendukung api direktori v 1.0 yang diperlukan?**

Microsoft graph adalah API yang direkomendasikan untuk direktori, identitas, dan manajemen akses. Namun, masih ada beberapa celah di antara apa yang dimungkinkan di Azure AD graph dan Microsoft graph. Tinjau artikel berikut, yang menyoroti perbedaan paling terkini untuk membantu pilihan Anda:

- [Perbedaan tipe sumber daya antara grafik Azure AD dan Microsoft graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Perbedaan properti antara Azure AD graph dan Microsoft graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Perbedaan metode antara Azure AD dan Microsoft graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**API yang saya panggil tidak berfungsi-di mana saya bisa melakukan lebih banyak pengujian?**

**Microsoft graph Explorer** -uji Microsoft graph api di penyewa Anda atau penyewa demo dan juga lihat **kueri sampel** di Microsoft graph Explorer.

**Aplikasi saya terlalu lambat dan juga mengalami kelambatan. Penyempurnaan apa yang bisa saya lakukan?**

Bergantung pada skenario Anda, ada berbagai opsi yang Anda inginkan untuk membuat aplikasi Anda lebih performant, dan dalam beberapa kasus, tidak rentan mengalami kelambatan oleh layanan (saat Anda membuat terlalu banyak panggilan).

- [Praktik terbaik Microsoft graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Permintaan pengelompokan](https://docs.microsoft.com/graph/json-batching)
- [Lacak perubahan melalui Delta query](https://docs.microsoft.com/graph/delta-query-overview)
- [Dapatkan pemberitahuan perubahan melalui webhooks](https://docs.microsoft.com/graph/webhooks)
- [Panduan pembatasan](https://docs.microsoft.com/graph/throttling)

**Di mana saya bisa menemukan informasi selengkapnya tentang kesalahan dan masalah yang diketahui?**

- [Informasi respons kesalahan Microsoft graph](https://docs.microsoft.com/graph/errors)
- [Masalah yang diketahui dengan Microsoft graph](https://docs.microsoft.com/graph/known-issues)

**Di mana saya dapat memeriksa status ketersediaan dan konektivitas Layanan?**

Ketersediaan layanan dan konektivitas layanan yang mendasari yang bisa diakses melalui Microsoft graph bisa berdampak pada ketersediaan dan kinerja keseluruhan Microsoft graph.

- Untuk kesehatan layanan direktori aktif Azure, Periksa status layanan **identitas + keamanan** yang tercantum di [halaman status Azure](https://azure.microsoft.com/status/).
- Untuk layanan Office yang berkontribusi ke Microsoft graph, Periksa status layanan yang tercantum di [dasbor Kesehatan Layanan Office](https://portal.office.com/adminportal/home#/servicehealth).

Kesalahan otorisasi Microsoft graph dapat berupa hasil dari beberapa masalah yang berbeda, yang sebagian besar menghasilkan kesalahan 401 atau 403. Misalnya, Semua hal berikut ini dapat menyebabkan kesalahan otorisasi:

- Kesalahan [aliran akuisisi token akses](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- [Lingkup izin](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) dikonfigurasi dengan buruk
- Kurangnya [persetujuan](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

**_Akhir dukungan untuk Pustaka Autentikasi Azure Active Directory (ADAL) dan API Grafik Azure AD (Grafik AAD)_* _

_ * Mulai 30 Juni 2020 * *, kami tidak akan lagi menambahkan fitur baru untuk ADAL dan Azure AD graph. Kami akan terus menyediakan dukungan teknis dan pembaruan keamanan, namun tidak akan lagi menyediakan pembaruan fitur.

**Mulai 30 juni 2022**, kami akan mengakhiri dukungan untuk ADAL dan Azure AD graph dan tidak akan lagi menyediakan dukungan teknis atau pembaruan keamanan.

Aplikasi yang menggunakan ADAL pada versi OS yang sudah ada akan terus berfungsi setelah waktu ini tetapi tidak akan *mendapatkan dukungan teknis atau pembaruan keamanan apa pun*.

Aplikasi menggunakan grafik Azure AD setelah waktu ini mungkin tidak lagi menerima respons dari titik akhir Azure AD graph.

**Migrasi ADAL**

Kami merekomendasikan Anda memperbarui ke [Pustaka Autentikasi Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), yang memiliki fitur dan pembaruan keamanan terbaru.

Jika Anda menggunakan Microsoft Apps, Ketahuilah bahwa Microsoft sedang dalam proses migrasi aplikasinya ke MSAL dengan tenggat waktu dukungan akhir, memastikan mereka akan mendapatkan manfaat dari peningkatan keamanan dan fitur yang sedang berlangsung.

1. [Baca FAQ ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Pelajari tentang cara melakukan migrasi aplikasi pada basis per platform](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Jika Anda memerlukan bantuan untuk memahami aplikasi mana yang menggunakan ADAL, kami menyarankan agar Anda meninjau semua kode sumber aplikasi Anda, dan jika ada, hubungi penyedia ISVs atau aplikasi apa pun. Dukungan Microsoft juga dapat menyediakan daftar semua aplikasi non-Microsoft ADAL di penyewa Anda.

**Migrasi Grafik AAD**

Untuk aplikasi yang menggunakan Azure AD graph, ikuti panduan kami untuk melakukan [migrasi aplikasi AZURE AD graph ke Microsoft graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).

1. [Daftar periksa migrasi kami menyediakan poin memulai](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. Portal pendaftaran aplikasi Azure Anda memperlihatkan aplikasi mana yang menggunakan Grafik AAD. Kami menyarankan Anda meninjau semua kode sumber aplikasi, dan jika memungkinkan, hubungi semua ISV atau penyedia aplikasi. Dukungan Microsoft juga bisa memberi Anda daftar semua penggunaan grafik AAD dalam penyewa Anda.
3. Agar aplikasi Anda dapat mengakses data di Microsoft graph, pengguna atau administrator harus memberinya izin yang benar melalui proses persetujuan. [Referensi izin Microsoft graph](https://docs.microsoft.com/graph/permissions-reference) mencantumkan izin yang terkait dengan setiap kumpulan utama api Microsoft graph. Ini juga memberikan panduan tentang cara menggunakan izin.
