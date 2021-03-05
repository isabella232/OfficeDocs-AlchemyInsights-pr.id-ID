---
title: Mengonfigurasi Layanan penyediaan
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
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482870"
---
# <a name="configuring-the-provision-service"></a>Mengonfigurasi Layanan penyediaan

Untuk penyediaan pengguna otomatis agar berfungsi, Azure AD memerlukan kredensial yang valid yang memungkinkan untuk menyambungkan ke Workday Web Services API. Selain itu, tombol uji koneksi pada hari kerja ke aplikasi penyediaan pengguna AD juga memvalidasi jika dapat tersambung ke agen bawaan Azure AD Connect yang terkait dengan domain AD.

Jika Azure portal mengembalikan kesalahan saat menyimpan kredensial, ikuti langkah-langkah di bawah ini:

1. Konfirmasi bahwa Anda telah mengonfigurasi akun pengguna sistem integrasi kerja seperti yang dinyatakan dalam bagian tutorial [mengonfigurasikan pengguna sistem integrasi di workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).
2. Konfirmasi bahwa layanan agen Azure AD Connect bawaan sudah aktif dan berjalan di server Windows lokal Anda menggunakan konsol Manajemen Layanan. Anda juga bisa memeriksa status agen di portal Azure dengan mengklik tombol Tampilkan agen lokal.
3. Pastikan bahwa Anda memasukkan nilai untuk bidang "nama pengguna Workday" menggunakan nama username@workday-penyewa format. Jika nama kerja-penyewa tidak hilang, maka hari kerja autentikasi gagal.
4. Jika Anda mengonfigurasi integrasi dengan penyewa implementasi hari kerja, perhatikan jam henti terjadwal dari penyewa hari kerja Anda. Workday telah menjadwalkan waktu untuk penyewa pelaksanaannya selama akhir pekan (biasanya dari Jumat sore hingga Sabtu pagi) dan kegagalan konektivitas selama jendela downtime ini adalah masalah umum yang diselesaikan secara otomatis segera setelah penyewa pelaksana kembali online.
5. Dalam kasus yang jarang, Anda mungkin juga melihat kesalahan ini jika kata sandi pengguna sistem integrasi berubah karena refresh penyewa atau jika akun tersebut dalam status dikunci atau kedaluwarsa. Periksa status pengguna sistem integrasi dengan administrator Workday Anda.

Untuk detail selengkapnya tentang mengonfigurasi workday untuk penyediaan otomatis, lihat [Tutorial: mengonfigurasi workday untuk penyediaan pengguna otomatis](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).
