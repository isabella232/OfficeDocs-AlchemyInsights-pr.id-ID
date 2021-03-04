---
title: Masalah dengan pengguna tunggal
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
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430210"
---
# <a name="problem-with-single-user"></a>Masalah dengan pengguna tunggal

- Pengguna mungkin belum ditetapkan karena layanan tidak memiliki kesempatan untuk mengevaluasi pengguna. Tinjau panduan cara penyediaan jangka panjang serta bilah kemajuan pada halaman konfigurasi bawaan. Jika status tetap ditentukan dalam bagian detail tambahan sebelum tanggal pengguna dibuat/diperbarui/dihapus, artinya kami belum mengevaluasi pengguna. Dalam skenario ini, hal terbaik yang harus dilakukan adalah menunggu Layanan penyediaan untuk menyelesaikan.

  - Perhatikan bahwa layanan kami hanya mengetahui perubahan pada pengguna di sistem sumber (Cloud HR). Harus ada perubahan yang valid dalam sistem sumber untuk Azure AD untuk mendeteksi perubahan dan alur ke direktori aktif.
- Layanan penyediaan dievaluasi pengguna dan ditentukan tidak boleh ditetapkan:
  - Jika Anda telah mengatur filter pelingkupan atribut berbasis, pastikan bahwa pengguna memenuhi kriteria yang telah Anda tentukan.
  - Jika pengguna sudah ada di sistem target dan status pengguna dalam kecocokan sumber dan target, kami tidak akan melakukan tindakan lebih lanjut.
- Layanan penyediaan berusaha untuk menyediakan pengguna dan gagal. Untuk skenario ini, Tinjau tab pemecahan masalah dan rekomendasi dari log penyediaan:
  - Atribut yang diperlukan pada pengguna mungkin hilang di direktori aktif di tempat atau Azure AD. Misalnya, aturan pembuatan userPrincipalName atau sAMAccountName tidak menghasilkan nilai yang tepat.
  - Atribut pencocokan (biasanya Idkaryawan) tidak mengatasi ke pengguna unik dalam direktori aktif di tempat atau Azure AD. Misalnya, ada dua pengguna dengan Idkaryawan yang sama di AD dan layanan mengembalikan kode kesalahan mengindikasikan entri target duplikat untuk entri sumber yang sama.

Untuk meninjau log untuk satu pengguna dan grup, lihat [meninjau log penyediaan masalah dengan pengguna tertentu](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).
