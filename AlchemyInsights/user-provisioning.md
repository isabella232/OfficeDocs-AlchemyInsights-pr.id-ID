---
title: Pengadaan pengguna
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
- "9004348"
- "8428"
ms.openlocfilehash: 12490df735ca8c524058404df92db79c6c5682fe2ecafe2b42baed70fa3ab142
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971342"
---
# <a name="user-provisioning"></a>Pengadaan pengguna

- Gunakan [kapabilitas penyediaan sesuai](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) permintaan untuk menyediakan pengguna dan mendapatkan diagnostik mendetail tentang langkah-langkah yang diambil.
- Untuk memecahkan masalah yang Anda temui saat menyediakan pengguna dan grup, lihat panduan pemecahan [masalah Tidak ada pengguna yang sedang disediakan.](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned)
- Jika Anda mengamati bahwa pengguna tidak tersedia, lihat Log [pengadaan (pratinjau) di](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) Azure Active Directory (AD). Mencari entri log yang berkaitan dengan pengguna tertentu.
- Secara berkala mulai ulang penyediaan untuk menemukan semua pengguna yang melewatkan di siklus penyediaan sebelumnya.
- Pengguna/grup mungkin belum tersedia karena layanan kami belum memiliki kesempatan untuk mengevaluasi pengguna. Tinjau panduan untuk waktu yang diperlukan penyediaan serta bilah kemajuan di halaman konfigurasi penyediaan. Jika status tetap yang ditentukan di bagian detail tambahan adalah sebelum tanggal pengguna dibuat/diperbarui/dihapus, artinya kami belum mengevaluasi pengguna. Dalam skenario ini, hal terbaik untuk dilakukan adalah menunggu layanan penyediaan selesai. Jika status tetap telah dicapai, kami menyarankan Anda untuk melakukan mulai ulang dari UI di Portal Azure.
  - Perhatikan bahwa layanan kami hanya mengetahui perubahan pada pengguna/grup di sistem sumber (Azure Active Directory). Jika pengguna/grup dihapus secara langsung di aplikasi (misalnya, ServiceNow), kami tidak menyadari perubahan tersebut dan tidak mengembalikannya berdasarkan status pengguna di sistem sumber. Dalam skenario ini, paling baik memutar kembali perubahan secara langsung di aplikasi target.
- Layanan kami mengevaluasi pengguna/grup dan menentukannya tidak boleh disediakan:
  - Jika Anda telah menetapkan lingkup untuk pengguna dan grup yang ditetapkan, periksa apakah pengguna/grup ditetapkan untuk aplikasi.
  - Jika pengguna/grup ditetapkan pada aplikasi, pastikan bahwa mereka tidak ditetapkan pada peran akses default. Peran ini tidak dapat digunakan untuk penyediaan.
  - Jika Anda telah menetapkan filter penjedaan berbasis atribut, pastikan pengguna memenuhi kriteria yang telah Anda tentukan.
  - Jika pengguna sudah ada dalam sistem target dan status pengguna di kecocokan sumber dan target, kami tidak akan melakukan tindakan lebih lanjut.
- Layanan kami berusaha menyediakan pengguna dan layanan tersebut gagal. Untuk skenario ini, tinjau tab pemecahan masalah dan rekomendasi dari log penyediaan:
  - Atribut yang diperlukan pada pengguna mungkin hilang di Azure Active Directory atau tidak cocok dengan format yang diperlukan oleh aplikasi pihak ketiga. Misalnya, atribut Negara pada pengguna mungkin diatur ke Amerika Serikat ketika harus merupakan AS.
  - Atribut adalah atribut referensial yang belum ada dalam aplikasi target. Atribut referensial adalah atribut yang menunjuk ke objek lain, misalnya, pengguna yang merupakan anggota dari grup. ID pengguna akan berada di atribut anggota grup, tetapi hanya dapat diproses jika objek pengguna yang di menunjuknya sudah ada.
