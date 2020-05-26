---
title: Jalankan Windows Memory Diagnostics di Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 3fedc52d02f1f70743429d0313eda0361306c3f3
ms.sourcegitcommit: 18b080c2a5d741af01ec589158effc35ea7cf449
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/19/2020
ms.locfileid: "44357790"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Jalankan Windows Memory Diagnostics di Windows 10

Jika Windows dan aplikasi pada PC Anda menabrak, pembekuan, atau bertindak dengan cara yang tidak stabil, Anda mungkin memiliki masalah dengan memori PC (RAM). Anda dapat menjalankan Windows Memory Diagnostic untuk memeriksa masalah dengan RAM PC.

Di kotak pencarian pada taskbar, ketik **diagnostik memori**, dan kemudian pilih **Windows Memory Diagnostic**. 

Untuk menjalankan diagnostik, PC harus me-restart. Anda memiliki pilihan untuk me-restart segera (silahkan menyimpan pekerjaan Anda dan menutup dokumen terbuka dan e-mail pertama), atau menjadwalkan diagnostik untuk menjalankan secara otomatis pada saat PC restart berikutnya:

![Diagnostik memori Windows](media/windows-memory-diagnostic.png)

Ketika PC dimulai ulang, **alat diagnostik memori Windows** akan berjalan secara otomatis. Status dan kemajuan akan ditampilkan sebagai menjalankan diagnostik, dan Anda memiliki pilihan untuk membatalkan diagnostik dengan menekan tombol **ESC** pada keyboard Anda.

Ketika diagnostik selesai, Windows akan mulai normal.
Segera setelah restart, saat desktop muncul, pemberitahuan akan muncul (di sebelah ikon **Action Center** pada taskbar), untuk menunjukkan apakah ada kesalahan memori yang ditemukan. Misalnya:

Inilah ikon Action Center: ![Ikon pusat aksi](media/action-center-icon.png) 

Dan contoh pemberitahuan: ![Tidak ada kesalahan memori](media/no-memory-errors.png)

Jika Anda melewatkan pemberitahuan, Anda dapat memilih ikon **pusat aksi** di taskbar untuk menampilkan **pusat aksi** dan melihat daftar pemberitahuan digulir.

Untuk meninjau informasi rinci, ketik **peristiwa** ke kotak pencarian di bilah tugas, dan kemudian pilih **peraga peristiwa**. Di panel sebelah kiri **penampil acara**, navigasikan ke **log Windows > sistem**. Di panel sebelah kanan, Pindai daftar sambil melihat kolom **sumber** , sampai Anda lihat peristiwa dengan nilai sumber **memorydiagnostics-hasil**. Sorot setiap acara tersebut dan lihat informasi hasil di kotak di bawah tab **umum** di bawah daftar.
