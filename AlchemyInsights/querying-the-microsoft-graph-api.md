---
title: Kueri API Microsoft graph
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
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974421"
---
# <a name="querying-the-microsoft-graph-api"></a>Kueri API Microsoft graph

Topik ini juga mungkin berlaku untuk pengembang masih menggunakan Azure AD graph API. Namun, **sangat disarankan agar** Anda menggunakan Microsoft graph untuk semua skenario manajemen direktori, identitas, dan akses Anda.

**Masalah autentikasi atau otorisasi**

- Jika aplikasi Anda **tidak dapat memperoleh token** untuk menghubungi Microsoft graph, pilih **masalah dengan mendapatkan kategori token Access (autentikasi)** Microsoft graph untuk mendapatkan bantuan dan dukungan yang lebih spesifik tentang topik ini.
- Jika aplikasi Anda **menerima kesalahan otorisasi 401 atau 403** saat memanggil Microsoft graph, pilih kategori Dapatkan Microsoft graph **error (otorisasi) Access ditolak (Authorization)** untuk mendapatkan bantuan dan dukungan yang lebih spesifik tentang topik ini.

**Saya ingin menggunakan Microsoft graph, tapi tidak yakin di mana memulai**

Untuk mempelajari selengkapnya tentang Microsoft graph, lihat:

- [Gambaran Umum Microsoft graph](https://docs.microsoft.com/graph/overview)
- [Gambaran umum manajemen identitas dan akses di Microsoft graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Membuat aplikasi Microsoft graph yang mulai](https://docs.microsoft.com/graph/)
- **Microsoft graph Explorer** -uji Microsoft graph api dalam penyewa atau penyewa demo Anda

**Saya ingin menggunakan Microsoft graph, tetapi apakah aplikasi ini mendukung api direktori v 1.0 yang diperlukan?**

Microsoft graph adalah API yang direkomendasikan untuk direktori, identitas, dan manajemen akses. Namun, masih ada beberapa celah di antara apa yang dimungkinkan di Azure AD graph dan Microsoft graph. Tinjau artikel berikut, yang menyoroti perbedaan paling terkini untuk membantu pilihan Anda:

- [Perbedaan tipe sumber daya antara grafik Azure AD dan Microsoft graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Perbedaan properti antara Azure AD graph dan Microsoft graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Perbedaan metode antara Azure AD dan Microsoft graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Saat saya meminta objek *pengguna* , banyak propertinya yang hilang**

`GET https://graph.microsoft.com/v1.0/users` hanya mengembalikan 11 properti, karena Microsoft graph otomatis memilih sekumpulan properti *pengguna* default untuk dikembalikan. Jika Anda memerlukan properti *pengguna* lain, gunakan $Select untuk memilih properti yang diperlukan aplikasi Anda. Cobalah di **Microsoft graph Explorer** terlebih dahulu.

**Beberapa nilai properti pengguna *kosong* meskipun saya tahu bahwa mereka sudah siap**

Penjelasan yang paling mungkin adalah bahwa aplikasi telah diberikan *pengguna. ReadBasic. All* permission. Hal ini memungkinkan aplikasi untuk membaca serangkaian properti pengguna, mengembalikan semua properti lain sebagai null meskipun telah ditetapkan sebelumnya. Coba Berikan izin kepada *pengguna aplikasi. baca. All* .

Untuk informasi selengkapnya, lihat [izin pengguna Microsoft graph](https://docs.microsoft.com/graph/permissions-reference#user-permissions).

**Saya mengalami masalah dalam menggunakan parameter kueri OData untuk memfilter data dalam permintaan saya**

Sementara Microsoft graph mendukung berbagai parameter kueri OData, banyak parameter tersebut yang tidak sepenuhnya didukung oleh layanan direktori (sumber daya yang mewarisi dari *Directoryobject*) di Microsoft graph. Batasan yang sama yang ada di grafik Azure AD tetap ada untuk sebagian besar di Microsoft graph:

1. **Tidak didukung**: $count, $Search, dan $filter nilai *null* atau *not null*
2. **Tidak didukung**: $filter pada properti tertentu (lihat topik sumber daya properti yang dapat difilter)
3. **Tidak didukung**: paging, pemfilteran, dan pengurutan pada saat yang sama
4. **Tidak didukung**: pemfilteran pada hubungan. Misalnya-Temukan semua anggota grup teknik yang ada di Inggris.
5. **Dukungan parsial**: $orderby pada *pengguna* (DisplayName dan userPrincipalName saja) dan *grup*
6. **Dukungan parsial**: $filter (hanya mendukung dukungan *EQ*, *startswith*, *or*, *and*, dan terbatas *apa pun*), $Expand (memperluas hubungan satu objek mengembalikan semua hubungan, tapi memperluas kumpulan hubungan objek)

Untuk informasi selengkapnya, lihat [mengkustomisasi respons dengan parameter kueri](https://docs.microsoft.com/graph/query-parameters).

**API yang saya panggil tidak berfungsi-di mana saya bisa melakukan lebih banyak pengujian?**

**Microsoft graph Explorer** -uji Microsoft graph api di penyewa Anda atau penyewa demo dan juga lihat **kueri sampel** di Microsoft graph Explorer.

**Saat saya meminta data sepertinya saya mendapatkan kumpulan data yang tidak lengkap kembali**

Jika Anda membuat kueri kumpulan (seperti *pengguna*), Microsoft graph menggunakan batas halaman sisi server sehingga hasilnya selalu dikembalikan dengan ukuran halaman default. Aplikasi Anda harus selalu menunggu untuk menelusuri kumpulan yang dikembalikan dari layanan.

Untuk informasi selengkapnya, lihat:

- [Praktik terbaik Microsoft graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Paging data Microsoft graph di aplikasi Anda](https://docs.microsoft.com/graph/paging)

**Aplikasi saya terlalu lambat dan juga mengalami kelambatan. Penyempurnaan apa yang bisa saya lakukan?**

Bergantung pada skenario Anda, ada berbagai opsi yang berbeda yang Anda inginkan untuk membuat aplikasi Anda lebih performant, dan dalam beberapa kasus, tidak rentan mengalami kelambatan oleh layanan (saat Anda membuat terlalu banyak panggilan).

Untuk mempelajari selengkapnya, lihat:

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
