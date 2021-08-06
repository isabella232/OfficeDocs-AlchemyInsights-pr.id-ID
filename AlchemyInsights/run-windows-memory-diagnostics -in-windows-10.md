---
title: Menjalankan Windows Diagnostik Memori di Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 63ba3afdd8f74b17559484f37e9250587aec9b4a929325d8f82e3c9ad06f1783
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53922544"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Menjalankan Windows Diagnostik Memori di Windows 10

Jika Windows dan aplikasi di PC Anda mengalami crash, berhenti berfungsi, atau bekerja dengan cara yang tidak stabil, Anda mungkin mengalami masalah dengan memori (RAM) PC. Anda dapat menjalankan Windows Diagnostik Memori untuk memeriksa masalah RAM PC.

Dalam kotak pencarian di taskbar Anda, ketik **diagnostik memori**, lalu pilih diagnostik Windows **Diagnostik Memori.** 

Untuk menjalankan diagnostik, PC harus dihidupkan ulang. Anda memiliki opsi untuk segera memulai ulang (silakan simpan pekerjaan dan tutup dokumen serta email yang terbuka terlebih dahulu), atau jadwalkan diagnostik untuk berjalan secara otomatis saat PC dimulai ulang di lain waktu:

![Windows Diagnostik Memori](media/windows-memory-diagnostic.png)

Saat PC dihidupkan ulang, Alat **Windows Diagnostik Memori akan** berjalan secara otomatis. Status dan kemajuan akan ditampilkan saat diagnostik berjalan, dan Anda memiliki opsi untuk membatalkan diagnostik dengan menekan **tombol ESC** di keyboard Anda.

Ketika diagnostik selesai, Windows akan dimulai secara normal.
Segera setelah mulai ulang, saat Desktop muncul, pemberitahuan  akan muncul (di samping ikon Pusat Tindakan di taskbar), untuk menunjukkan apakah ada kesalahan memori yang ditemukan. Misalnya:

Berikut ikon Pusat Tindakan: ![Ikon pusat tindakan](media/action-center-icon.png) 

Dan pemberitahuan sampel: ![Tidak ada kesalahan memori](media/no-memory-errors.png)

Jika Anda melewatkan pemberitahuan, Anda bisa memilih ikon **Pusat** Tindakan pada taskbar untuk menampilkan Pusat **Tindakan** dan melihat daftar pemberitahuan yang bisa digulir.

Untuk meninjau informasi mendetail, ketikkan **acara** ke dalam kotak pencarian di taskbar, lalu pilih **Penampil Kejadian**. Di panel **kiri Penampil** Kejadian, navigasikan ke Windows Log **> Sistem.** Di panel sebelah kanan, pindai daftar sambil  melihat kolom Sumber, hingga Anda melihat kejadian dengan nilai Sumber **MemoriDiagnostics-Hasil.** Sorot setiap kejadian tersebut dan lihat informasi hasilnya dalam kotak di bawah tab **Umum** di bawah daftar tersebut.
