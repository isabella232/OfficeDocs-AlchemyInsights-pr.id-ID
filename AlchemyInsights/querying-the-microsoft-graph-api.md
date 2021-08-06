---
title: Membuat kueri API Graph Microsoft
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
ms.openlocfilehash: eda5d8d1d76d0d87312b1441aeae89d8e250abe0e8b613d4a43fcc2345a6f021
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923242"
---
# <a name="querying-the-microsoft-graph-api"></a>Membuat kueri API Graph Microsoft

Topik ini mungkin juga berlaku untuk pengembang yang masih menggunakan API Azure AD Graph. Namun, sangat **dianjurkan agar** Anda menggunakan Microsoft Graph semua skenario manajemen direktori, identitas, dan akses.

**Masalah autentikasi atau otorisasi**

- Jika aplikasi Anda tidak dapat memperoleh **token** untuk menghubungi Microsoft Graph, pilih Masalah dengan mendapatkan token akses **(Autentikasi)** kategori Microsoft Graph untuk mendapatkan bantuan dan dukungan yang lebih spesifik tentang topik ini.
- Jika aplikasi Anda menerima **401 atau 403** kesalahan otorisasi saat menghubungi Microsoft Graph, pilih kategori Mendapatkan akses yang ditolak **(Otorisasi)** API Microsoft Graph untuk mendapatkan bantuan dan dukungan yang lebih spesifik tentang topik ini.

**Saya ingin menggunakan Microsoft Graph, tetapi tidak yakin harus memulai dari mana**

Untuk mempelajari selengkapnya tentang Microsoft Graph, lihat:

- [Gambaran umum Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Gambaran umum tentang Identitas dan Manajemen Akses di Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Mulai membangun aplikasi Microsoft Graph baru](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** - Uji Graph API Microsoft di penyewa Anda atau penyewa demo

**Saya ingin menggunakan Microsoft Graph, tapi apakah aplikasi ini mendukung API direktori v1.0 yang saya perlukan?**

Microsoft Graph adalah API yang disarankan untuk manajemen direktori, identitas, dan akses. Namun, masih ada beberapa jarak antara apa yang mungkin dilakukan di Azure AD Graph dan Microsoft Graph. Tinjau artikel berikut, yang menyoroti perbedaan yang paling baru untuk membantu dalam pilihan Anda:

- [Perbedaan tipe sumber daya antara Azure AD Graph dan Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Perbedaan properti antara Azure AD Graph dan Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Perbedaan metode antara Azure AD dan Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Saat saya membuat kueri *objek* pengguna, banyak propertinya yang hilang**

`GET https://graph.microsoft.com/v1.0/users`hanya mengembalikan 11 properti, karena Microsoft Graph otomatis memilih kumpulan properti *pengguna* default untuk dikembalikan. Jika Anda membutuhkan properti *pengguna* yang lain, $select untuk memilih properti yang dibutuhkan aplikasi Anda. Coba di **Microsoft Graph Explorer terlebih** dahulu.

**Beberapa nilai properti pengguna *null* meskipun saya tahu nilai tersebut sudah ditetapkan**

Penjelasan paling mungkin adalah bahwa aplikasi telah diberikan izin *User.ReadBasic.All.* Hal ini memungkinkan aplikasi untuk membaca kumpulan properti pengguna terbatas, yang mengembalikan semua properti lainnya sebagai null meskipun telah diatur sebelumnya. Coba berikan aplikasi izin *User.Read.All.*

Untuk informasi selengkapnya, lihat [Microsoft Graph izin pengguna](https://docs.microsoft.com/graph/permissions-reference#user-permissions).

**Saya mengalami masalah dalam menggunakan parameter kueri OData untuk memfilter data dalam permintaan saya**

Saat Microsoft Graph mendukung rentang parameter kueri OData yang luas, banyak dari parameter tersebut tidak sepenuhnya didukung oleh layanan direktori (sumber daya yang mewarisi dari *directoryObject*) di Microsoft Graph. Batasan yang sama seperti yang ada di Azure AD Graph akan tetap ada untuk sebagian besar bagian di Microsoft Graph:

1. **Tidak didukung :**$count, $search, dan $filter nilai *null* *atau bukan* null
2. **Tidak didukung**: $filter properti tertentu (lihat topik sumber daya di properti mana yang dapat difilter)
3. **Tidak didukung**: paging, pemfilteran, dan pengurutan pada saat yang sama
4. **Tidak didukung**: pemfilteran pada hubungan. Misalnya - menemukan semua anggota grup teknik yang ada di Inggris.
5. **Dukungan sebagian**: $orderby *pada pengguna* (displayName dan userPrincipalName saja) dan *grup*
6. **Dukungan sebagian**: $filter (hanya mendukung *eq*, *startswith* *,* atau *,* dan , dan limited *any*) support, $expand (memperluas hubungan objek tunggal yang mengembalikan semua hubungan, namun memperluas kumpulan hubungan objek terbatas)

Untuk informasi selengkapnya, [lihat Mengustomisasi respons dengan parameter kueri](https://docs.microsoft.com/graph/query-parameters).

**API yang saya panggil tidak berfungsi - di mana saya bisa melakukan lebih banyak pengujian?**

**Microsoft Graph Explorer** - Uji api Graph Microsoft dalam penyewa atau penyewa demo dan lihat juga contoh **kueri** di Microsoft Graph Explorer.

**Saat saya membuat kueri untuk data, tampaknya saya mendapatkan kumpulan data yang tidak lengkap**

If you are querying a collection (like *users*), Microsoft Graph uses server-side page limits so results are always returned with a default page-size. Aplikasi Anda seharusnya selalu melihat setiap kumpulan yang dikembalikan dari layanan.

Untuk informasi selengkapnya, lihat:

- [Praktik Graph terbaik Microsoft](https://docs.microsoft.com/graph/best-practices-concept)
- [Data data Graph Microsoft dalam aplikasi Anda](https://docs.microsoft.com/graph/paging)

**Aplikasi saya terlalu lambat dan juga tidak dapat digunakan. Penyempurnaan apa yang dapat saya buat?**

Bergantung pada skenario Anda, ada berbagai opsi berbeda menurut Anda untuk membuat aplikasi Anda lebih berkinerja, dan dalam beberapa kasus, lebih sedikit rentan terhadap yang terbatas oleh layanan (ketika Anda melakukan terlalu banyak panggilan).

Untuk mempelajari selengkapnya, lihat:

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
