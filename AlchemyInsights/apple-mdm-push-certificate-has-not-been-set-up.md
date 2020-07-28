---
title: Apple MDM push Certificate belum diatur
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439381"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a>Apple MDM push Certificate belum diatur

Apple MDM push Certificate (juga dikenal sebagai sertifikat Layanan pemberitahuan push Apple (APNS)) belum dikonfigurasi untuk langganan Anda. Tanpa sertifikat push MDM Apple yang dikonfigurasi, Anda tidak dapat mendaftarkan dan mengelola perangkat iOS dan Mac OS. Setelah Anda menambahkan sertifikat untuk Intune, pengguna dapat menginstal aplikasi portal perusahaan untuk mendaftarkan perangkat iOS.

1. Pilih **"Saya setuju."** untuk memberikan izin kepada Microsoft untuk mengirim data ke Apple.

2. Pilih **Download CSR Anda** Intune penandatanganan sertifikat permintaan yang diperlukan untuk membuat Apple Mdm push Certificate. File tersebut digunakan untuk meminta sertifikat hubungan kepercayaan dari portal sertifikat push Apple.

3. Pilih **buat Mdm push Certificate Anda** untuk membuka Apple push Certificates portal. Masuk dengan ID Apple perusahaan Anda, lalu pilih **buat sertifikat**. Pilih **Pilih file**, Jelajahi file permintaan penandatanganan sertifikat, lalu pilih **Unggah**. Pada halaman konfirmasi, pilih **Download** untuk mendownload file Certificate (. pem), dan simpan file secara lokal.
 
**Catatan**: sertifikat ini DIKAITKAN dengan ID Apple yang digunakan untuk membuatnya. Sebagai praktik terbaik, gunakan ID Apple perusahaan untuk tugas manajemen, dan pastikan kotak pesan dipantau oleh lebih dari satu orang atau dengan menggunakan daftar distribusi. Jangan gunakan ID Apple pribadi. Gunakan ID Apple yang sama untuk memperbarui Apple push Certificate setiap 12 bulan.
 
4. Masukkan ID Apple yang digunakan untuk membuat sertifikat push Apple MDM. Catat ID ini sebagai pengingat saat Anda perlu memperpanjang sertifikat.

5. Buka file Certificate (. pem), pilih **Open**, lalu pilih **upload**. Dengan sertifikat push, Intune dapat mendaftarkan dan mengelola perangkat Apple.