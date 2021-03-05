---
title: Penyediaan pengguna
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
ms.openlocfilehash: bd415b2d44bccf0c2b3eccb4e38452498b748b3a
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481888"
---
# <a name="user-provisioning"></a>Penyediaan pengguna

- Gunakan kemampuan [penyediaan sesuai permintaan](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) untuk menyediakan pengguna dan Dapatkan diagnosa mendetail tentang langkah-langkah yang diambil.
- Untuk memecahkan masalah yang Anda hadapi saat menyediakan pengguna dan grup, lihat panduan pemecahan masalah [tidak ada pengguna yang ditetapkan](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned).
- Jika Anda mengamati bahwa pengguna tidak tersedia, lihat [log penyediaan (pratinjau)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) di Azure Active Directory (AD). Mencari entri log yang berkaitan dengan pengguna tertentu.
- Mulai ulang penyediaan secara berkala untuk menangkap pengguna yang tidak terjawab dalam siklus penyediaan sebelumnya.
- Pengguna/grup mungkin belum ditetapkan karena layanan kami tidak memiliki kesempatan untuk mengevaluasi pengguna. Tinjau panduan cara penyediaan jangka panjang serta bilah kemajuan pada halaman konfigurasi bawaan. Jika status tetap ditentukan dalam bagian detail tambahan sebelum tanggal pengguna dibuat/diperbarui/dihapus, artinya kami belum mengevaluasi pengguna. Dalam skenario ini, hal terbaik yang harus dilakukan adalah menunggu Layanan penyediaan untuk menyelesaikan. Jika status mapan telah tercapai, kami menyarankan untuk melakukan mulai ulang dari UI di portal Azure.
  - Perhatikan bahwa layanan kami hanya mengetahui perubahan pada pengguna/grup di sistem sumber (Azure Active Directory). Jika pengguna/grup dihapus secara langsung dalam aplikasi (misalnya, ServiceNow), kami tidak mengetahui perubahan tersebut dan tidak menggulung kembali berdasarkan pada status pengguna di sistem sumber. Dalam skenario ini, sebaiknya gulung kembali perubahan secara langsung dalam aplikasi target.
- Layanan kami mengevaluasi pengguna/grup dan memutuskan bahwa tidak tersedia:
  - Jika Anda telah mengatur lingkup ke pengguna dan grup yang ditetapkan, periksa apakah pengguna/grup ditetapkan ke aplikasi tersebut.
  - Jika pengguna/grup ditetapkan ke aplikasi, pastikan mereka tidak ditetapkan ke peran akses default. Peran ini tidak dapat digunakan untuk penyediaan.
  - Jika Anda telah mengatur filter pelingkupan atribut berbasis, pastikan bahwa pengguna memenuhi kriteria yang telah Anda tentukan.
  - Jika pengguna sudah ada di sistem target dan status pengguna dalam kecocokan sumber dan target, kami tidak akan melakukan tindakan lebih lanjut.
- Layanan kami berusaha untuk menyediakan pengguna dan gagal. Untuk skenario ini, Tinjau tab pemecahan masalah dan rekomendasi dari log penyediaan:
  - Atribut yang diperlukan pada pengguna mungkin tidak ditemukan di Azure Active Directory atau tidak cocok dengan format yang diperlukan oleh aplikasi pihak ketiga. Misalnya, atribut Country di pengguna mungkin diatur ke Amerika Serikat saat harus menggunakan kami.
  - Atribut adalah atribut referensial yang belum ada dalam aplikasi target. Atribut referensial adalah atribut yang mengarahkan ke objek lain, misalnya, pengguna yang merupakan anggota grup. ID pengguna akan berada dalam atribut anggota grup, tetapi hanya dapat diproses jika objek pengguna yang telah ada di dalamnya.
