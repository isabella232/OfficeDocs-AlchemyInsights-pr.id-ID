---
title: Mengonfigurasi layanan Provisi
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: 271ab7ad34c0f85f6f5a9d8d3dc2d901fe6fe8f978a2cc98eed986f594036f17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54033281"
---
# <a name="configuring-the-provision-service"></a>Mengonfigurasi layanan Provisi

Agar penyediaan pengguna otomatis berfungsi, Azure AD memerlukan kredensial valid yang memungkinkannya tersambung ke API Layanan Web Workday. Lebih lanjut, tombol Uji Koneksi pada Hari Kerja ke aplikasi Penyediaan Pengguna AD juga memvalidasi apakah aplikasi dapat tersambung ke Agen Penyediaan Azure AD Koneksi yang terkait dengan Domain AD.

Jika portal Azure mengembalikan kesalahan saat menyimpan kredensial, ikuti langkah-langkah yang disarankan di bawah ini:

1. Konfirmasi bahwa Anda telah mengonfigurasi akun Pengguna Sistem Integrasi Hari Kerja seperti yang dinyatakan di bagian tutorial [Mengonfigurasi pengguna sistem integrasi di Hari Kerja.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
2. Pastikan bahwa Layanan Agen Koneksi Azure AD telah tersedia dan berjalan di server Windows lokal Anda menggunakan Konsol Manajemen Layanan. Anda juga dapat memeriksa status agen di portal Azure dengan mengklik tombol Tampilkan agen lokal.
3. Pastikan Anda memasukkan nilai untuk bidang "Nama Pengguna Hari Kerja" menggunakan format username@workday-nama-penyewa. Jika nama penyewa hari kerja hilang, Autentikasi hari kerja gagal.
4. Jika Anda mengonfigurasi integrasi dengan penyewa penerapan Hari Kerja, perhatikan jam henti terjadwal dari penyewa Hari Kerja Anda. Hari kerja telah menjadwalkan waktu turun untuk penerapan penyewa selama akhir pekan (biasanya dari Jumat malam hingga Sabtu pagi) dan kegagalan konektivitas selama jendela waktu henti ini merupakan masalah yang diketahui yang diatasi secara otomatis segera setelah penyewa implementasi kembali online.
5. Dalam kasus yang jarang terjadi, Anda mungkin juga melihat kesalahan ini jika kata sandi Pengguna Sistem Integrasi diubah karena refresh penyewa atau jika akun dalam status terkunci atau kedaluwarsa. Silakan periksa status pengguna Sistem Integrasi dengan administrator Hari Kerja Anda.

Untuk detail selengkapnya tentang mengonfigurasi hari kerja untuk penyediaan otomatis, lihat [Tutorial: Mengonfigurasi Hari Kerja untuk penyediaan pengguna otomatis.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
