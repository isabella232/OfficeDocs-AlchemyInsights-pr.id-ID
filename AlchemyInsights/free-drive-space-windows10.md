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
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036588"
---
# <a name="free-up-drive-space-in-windows-10"></a>Mengosongkan ruang drive di Windows 10

Berikut adalah dua opsi untuk mengosongkan ruang drive di Windows:

- Mengosongkan ruang drive di Windows 10.
- Mengosongkan ruang untuk pembaruan Windows 10 dengan perangkat penyimpanan eksternal.

Jika Anda masih memiliki ruang disk yang rendah setelah menggunakan pembersihan disk, ada kemungkinan folder Temp Anda mengisi dengan file Application (. Appx) yang digunakan oleh Microsoft Store. Untuk memperbaiki masalah ini, reset penyimpanan, kosongkan tembolok penyimpanan, lalu jalankan pemecah masalah pembaruan Windows. Pastikan Microsoft Store ditutup sebelum Anda melanjutkan langkah-langkah ini.

**Langkah 1: mereset Microsoft Store**

**Catatan** Ini menghapus data aplikasi secara permanen pada perangkat, termasuk preferensi dan detail masuk Anda.

1. Pilih **mulai**  >  **pengaturan**  >  **aplikasi** aplikasi  >  **& fitur**.

1. Di daftar aplikasi, temukan dan pilih Microsoft Store.

1. Pilih **opsi tingkat lanjut**.

1. Gulir ke bawah dan pilih **reset**, lalu **konfirmasikan ulang**.

**Langkah 2: Kosongkan singgahan penyimpanan Microsoft**

1. Tekan tombol logo Windows + R untuk membuka kotak dialog Jalankan.

1. Ketik wsreset.exe dan pilih **OK**.

1. Jendela prompt perintah kosong terbuka. Setelah sekitar 10 detik, jendela tertutup dan penyimpanan akan terbuka secara otomatis.

**Langkah 3: reset pembaruan Windows**

1. Pilih **mulai**  >  **pengaturan**  >  **pembaruan &**  >  **pemecahan masalah** keamanan.

1. Gulir ke bawah dan pilih **Windows Update** dari daftar, lalu pilih **Jalankan pemecah masalah**.

1. Hidupkan ulang komputer Anda dan periksa apakah Anda masih mengalami masalah tersebut.

