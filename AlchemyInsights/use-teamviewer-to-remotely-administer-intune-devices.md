---
title: Gunakan TeamViewer untuk mengelola perangkat Intune dari jarak jauh
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555240"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a>Gunakan TeamViewer untuk mengelola perangkat Intune dari jarak jauh

Perangkat yang dikelola oleh Intune dapat diberikan dari jarak jauh dengan menggunakan [TeamViewer](https://www.teamviewer.com/).

Untuk mengelola Intune menggunakan TeamViewer, gunakan langkah berikut: 

Mulailah dengan mendapatkan kredensial dari TeamViewer untuk mengatur konektor TeamViewer di Intune. Hal ini memungkinkan admin untuk memasukkan kredensial dalam TeamViewer Connector UI di bawah perangkat, operasi satu kali untuk menetapkan hubungan antara Intune dan layanan TeamViewer.

**Bagian 1: mulai sesi dengan perangkat jarak jauh**

1. Di bawah **semua perangkat**, pilih perangkat yang ingin Anda gunakan untuk memulai sesi jarak jauh.
2. Dari **... Lebih lanjut**, pilih **sesi bantuan jarak jauh baru**.
3. Pilih **ya** untuk mengetahui bahwa Anda ingin membuat sesi jarak jauh.
    Setelah permintaan "memulai sesi remote baru" diakui oleh layanan TeamViewer, Anda akan melihat opsi untuk **memulai bantuan jarak jauh** di bawah detail panel Ikhtisar (atau, penting) untuk perangkat. Pilih **Lihat lebih** untuk memperluas panel dan menampilkan status bantuan jarak jauh.
4. Pilih **mulai sesi jarak jauh** untuk memulai sesi di sisi admin.
5. Pilih untuk mengunduh biner TeamViewer (Windows), dan pilih **Jalankan**.<br/>
    **Catatan** Anda dapat mengabaikan halaman web browser yang dibuka ke situs web TeamViewer.

6. Akui permintaan Aplikasi TeamViewer untuk melakukan perubahan pada perangkat (khusus Windows).
7. Aplikasi TeamViewer dimulai dan mencakup kode sesi untuk mengotentikasi koneksi dengan perangkat remote.

**Bagian 2: pada perangkat yang ditargetkan untuk sesi jarak jauh**

1. Buka portal perusahaan Intune.
2. Cari bendera pemberitahuan: "administrator TI Anda meminta kontrol perangkat ini untuk sesi bantuan jarak jauh," dan pilih pemberitahuan.
3. Pilih untuk mengunduh aplikasi TeamViewer, atau Akui download aplikasi TeamViewer dari App Store, lalu pilih **Run**.
    **Catatan** Anda dapat mengabaikan halaman web browser yang dibuka ke situs web TeamViewer.

4. Akui permintaan Aplikasi TeamViewer untuk melakukan perubahan pada perangkat (khusus Windows).
5. Aplikasi TeamViewer dimulai dan mencakup kode sesi untuk mengotentikasi koneksi dengan perangkat remote.
6. Popup bertanya apakah Anda ingin mengizinkan sesi untuk memulai.

**Catatan** Kode sesi yang dihasilkan oleh layanan TeamViewer hanya digunakan satu kali. Jika sambungan terputus, Anda harus:

1. Tutup instance aplikasi TeamViewer di perangkat remote dan di Stasiun kerja admin.
2. Tutup portal perusahaan pada perangkat jauh.
3. Memulai baru "sesi bantuan remote baru" dari admin portal.
4. Membuka kembali portal perusahaan pada perangkat jauh untuk menerima pemberitahuan baru.
5. Unduh dan buka Aplikasi TeamViewer pada perangkat remote dan workstation admin, seperti sebelumnya.