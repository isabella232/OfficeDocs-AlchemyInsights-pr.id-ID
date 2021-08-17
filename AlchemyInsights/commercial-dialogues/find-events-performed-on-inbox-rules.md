---
title: Menemukan acara yang dilakukan pada aturan kotak masuk
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: d6a4eadd897dfae3b65ccda6363edfe9cef1c810
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/13/2021
ms.locfileid: "58313502"
---
# <a name="find-events-performed-on-inbox-rules"></a>Menemukan acara yang dilakukan pada aturan kotak masuk

Ketika aturan kotak masuk dibuat, diubah, atau dihapus, kejadian direkam dalam log audit. Berikut cara meninjaunya:

1. Lakukan salah satu tindakan berikut ini:
   - Pada pusat kepatuhan Microsoft 365 , <https://compliance.microsoft.com> masuk ke **Audit** \> **Solusi**. Atau, untuk langsung masuk ke **halaman Audit,** gunakan <https://compliance.microsoft.com/auditlogsearch> .
   - Pada portal Pertahanan Microsoft 365 di <https://security.microsoft.com> , masuk ke **Audit**. Atau, untuk langsung masuk ke **halaman Audit,** gunakan <https://security.microsoft.com/auditlogsearch> .

    **Catatan**: Jika melihat pemberitahuan bahwa Anda perlu mengaktifkan pengauditan, lanjutkan dan aktifkan sekarang. Jika fitur ini tidak diaktifkan, hasil pencarian tidak akan dapat mengambil data dari tanggal sebelumnya.
1. Pilih bidang Aktivitas dan temukan Exchange kotak surat Anda, lalu pilih New-InboxRule Membuat aturan kotak masuk dari Outlook Web App. Jika sudah selesai, klik di luar panel untuk meminimalkan panel Aktivitas.
1. Tentukan rentang tanggal, lalu di bidang Pengguna, pilih nama pengguna untuk pengguna yang ingin Anda selidiki. Anda bisa memilih lebih dari satu pengguna dalam satu waktu.
1. Pilih Pencarian. Aktivitas muncul di bawah Hasil.
1. Untuk melihat detail, pilih aktivitas, lalu pilih Informasi Selengkapnya. Di bawah bagian Parameter Anda bisa melihat nama aturan, kumpulan ketentuan, dan tindakan yang akan diambil aturan.

2. Pada tab **Pencarian** dari halaman **Audit,** konfigurasi pengaturan berikut ini:
   - **Rentang tanggal dan waktu**: Pilih rentang tanggal/waktu dalam **kotak** Mulai **dan** Akhir.
   - **Aktivitas**: Pilih **Aturan Kotak Masuk Baru Buat aturan kotak masuk Outlook Web App**

3. Bila Anda sudah selesai, klik **Cari.** Aktivitas akan muncul di halaman **Pencarian audit baru.**

4. Pilih aktivitas dalam hasil untuk membuka flyout detail. Di bawah **bagian** Parameter Anda bisa melihat nama aturan, kumpulan ketentuan, dan tindakan yang akan diambil aturan.

Untuk mempelajari selengkapnya, lihat [Mencari log audit untuk menyelidiki masalah dukungan umum.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
