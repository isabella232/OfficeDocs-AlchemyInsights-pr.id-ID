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
ms.openlocfilehash: 8d8821cda94b2af244fa317707421f9d197b6052fb316789cd286ea8b4adf19e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960154"
---
# <a name="problem-with-single-user"></a>Masalah dengan pengguna tunggal

- Pengguna mungkin belum ditetapkan karena layanan belum mempunyai kesempatan untuk mengevaluasi pengguna. Tinjau panduan untuk waktu yang diperlukan penyediaan serta bilah kemajuan di halaman konfigurasi penyediaan. Jika status tetap yang ditentukan di bagian detail tambahan adalah sebelum tanggal pengguna dibuat/diperbarui/dihapus, artinya kami belum mengevaluasi pengguna. Dalam skenario ini, hal terbaik untuk dilakukan adalah menunggu layanan penyediaan selesai.

  - Perhatikan bahwa layanan kami hanya mengetahui perubahan kepada pengguna di sistem sumber (CLOUD HR). Harus ada perubahan yang valid dalam sistem sumber bagi Azure AD untuk mendeteksi perubahan dan mengalirkan ke Direktori Aktif.
- Layanan pengadaan yang dievaluasi pengguna dan menentukannya tidak boleh diprovisikan:
  - Jika Anda telah menetapkan filter penjedaan berbasis atribut, pastikan pengguna memenuhi kriteria yang telah Anda tentukan.
  - Jika pengguna sudah ada dalam sistem target dan status pengguna di kecocokan sumber dan target, kami tidak akan melakukan tindakan lebih lanjut.
- Layanan penyedia berusaha menyediakan pengguna dan layanan tersebut gagal. Untuk skenario ini, tinjau tab pemecahan masalah dan rekomendasi dari log penyediaan:
  - Atribut yang diperlukan pada pengguna mungkin hilang di Direktori Aktif lokal atau Azure AD. Misalnya, aturan pembuatan userPrincipalName atau sAMAccountName tidak menghasilkan nilai yang tepat.
  - Atribut yang cocok (biasanya employeeId) tidak mengatasi masalah bagi pengguna unik dalam Active Directory lokal atau Azure AD. Misalnya, terdapat dua pengguna dengan ID karyawan yang sama pada AD dan layanan mengembalikan kode kesalahan yang menunjukkan entri target duplikat untuk entri sumber yang sama.

Untuk meninjau log untuk pengguna dan grup [tunggal, lihat Meninjau log provisi untuk masalah dengan pengguna tertentu.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)
