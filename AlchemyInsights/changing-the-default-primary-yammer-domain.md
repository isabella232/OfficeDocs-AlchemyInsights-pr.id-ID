---
title: Mengubah domain Yammer default
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002662"
- "5162"
ms.openlocfilehash: 6a7215ef7187e8dc6c834470b4724692b239efd4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817983"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a>Mengubah domain Yammer default/utama

URL Yammer berisi nama domain utama saat ini untuk jaringan Yammer Anda. Nama domain ini mungkin tidak sesuai dengan nama domain utama yang ditetapkan di Office 365 atau Azure AD. Terdapat perbedaan dalam perilaku berdasarkan jumlah domain kustom yang ditambahkan ke penyewa, dan apakah Yammer berada di konfigurasi yang didukung (1 Penyewa: 1 Jaringan, atau 1:1). Dokumentasi mengenai [Domain Yammer dan Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains) tersedia.

Alasan paling umum ketika Anda melihat domain yang salah adalah terdapat beberapa jaringan Yammer dan perlu dikonsolidasikan. [Mengonsolidasikan ke jaringan tunggal](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) menggunakan alat migrasi jaringan merupakan langkah pertama yang penting. Selesaikan langkah ini sebelum mencoba mengatur domain utama Anda.

**Tanpa domain kustom**

Untuk penyewa baru, domain default (misalnya fabrikam.onmicrosoft.com) dari penyewa akan digunakan untuk Yammer. Domain utama diatur ke yammer.com/fabrikam.onmicrosoft.com.

**Satu domain kustom**

Yammer akan secara otomatis memilih domain kustom (misalnya fabrikam.com) dari penyewa sebagai domain utama di Yammer. Domain ini diatur ke yammer.com/fabrikam.com. Perubahan ini dibuat oleh layanan sinkronisasi domain, dan dapat memakan waktu hingga 24 jam untuk diterapkan.

**Beberapa domain kustom**

Yammer dapat memiliki domain utama yang berbeda dari domain penyewa default. Karena ada beberapa domain kustom, Yammer tidak berupaya untuk menebak domain yang benar dari yang tersedia. Anda perlu membuka kasus dukungan untuk meminta nama domain utama diubah ke domain utama pilihan Anda.

**Informasi pemecahan masalah tambahan**

Dalam beberapa kasus, domain mungkin telah berpindah di antara penyewa dan layanan sinkronisasi domain belum berhasil dijalankan. Anda mungkin mengalami masalah masuk atau yang lainnya, selain masalah domain utama yang tidak benar. Untuk mengatasi masalah ini, domain mungkin perlu dipindahkan ke jaringan yang benar dengan bantuan dari Dukungan Microsoft. Situasi ini memerlukan bantuan langsung dan dapat memakan waktu agak lama untuk mengatasinya, terutama jika daftar nama domainnya sangat panjang. Buka kasus dukungan untuk mendapatkan bantuan dalam mengatasi masalah semacam ini.

Saat bekerja dengan agen dukungan, mereka akan memeriksa bahwa domain diverifikasi pada penyewa di bawah kontrol Anda. Mereka mungkin akan mengajukan pertanyaan verifikasi tambahan tentang domain Anda jika domain tersebut ditambahkan ke penyewa tetapi tidak diverifikasi oleh DNS. Pastikan domain diverifikasi oleh DNS untuk mempercepat prosesnya.
