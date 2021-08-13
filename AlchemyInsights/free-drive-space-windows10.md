---
title: Mengosongkan ruang drive di Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: c7d29ab718be8dbdcde61a7de2f158fb3bbd722d2964d8b13cde9936dd1e5ee1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53928084"
---
# <a name="free-up-drive-space-in-windows-10"></a>Mengosongkan ruang drive di Windows 10

Ada dua opsi untuk mengosongkan ruang drive di Windows:

- Mengosongkan ruang drive di Windows 10.
- Kosongkan ruang untuk pembaruan Windows 10 dengan perangkat penyimpanan eksternal.

Jika ruang disk masih rendah setelah menggunakan Pembersihan Disk, kemungkinan folder Temp Anda dengan cepat terisi file aplikasi (.appx) yang digunakan oleh Microsoft Store. Untuk memperbaiki masalah ini, atur ulang Store, bersihkan cache Store, lalu jalankan pemecah masalah Windows Update. Pastikan Microsoft Store ditutup sebelum Anda melanjutkan ke langkah-langkah berikut.

**Langkah 1: Atur ulang Microsoft Store**

**Catatan** Tindakan ini akan menghapus permanen data aplikasi di perangkat, termasuk preferensi Anda dan detail masuk.

1. Pilih **Mulai** > **Pengaturan** > **Aplikasi** > **Aplikasi & fitur**.

1. Di daftar aplikasi, temukan dan pilih Microsoft Store.

1. Pilih **Opsi lanjutan**.

1. Gulir ke bawah dan pilih **Atur Ulang**, lalu **Konfirmasi Atur Ulang**.

**Langkah 2: Bersihkan cache Microsoft Store**

1. Tekan Tombol Logo Windows + R untuk membuka Jalankan kotak dialog.

1. Ketik wsreset.exe lalu pilih **OK**.

1. Jendela Perintah kosong akan terbuka. Setelah sekitar 10 detik, jendela tersebut akan tertutup dan Store akan terbuka secara otomatis.

**Langkah 3: Atur Ulang Windows Update**

1. Pilih **Mulai** > **Pengaturan** > **Pembaruan & Keamanan** > **Pemecahan Masalah**.

1. Gulir ke bawah dan pilih **Windows Update** dari daftar, lalu pilih **Jalankan pemecah masalah**.

1. Boot ulang komputer, lalu periksa apakah Anda masih mengalami masalah tersebut.

