---
title: Membaca log audit untuk kejadian yang dihapus
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
ms.openlocfilehash: ec8f845f599e397814bc9077c3fe59edb5324192
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324736"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>Membaca log audit untuk kejadian yang dihapus

Berikut cara melakukannya:

1. Lakukan salah satu tindakan berikut ini:
   - Pada bagian pusat kepatuhan Microsoft 365 <https://compliance.microsoft.com> , masuk ke **Audit** \> **Solusi**. Atau, untuk langsung masuk ke **halaman Audit,** gunakan <https://compliance.microsoft.com/auditlogsearch> .
   - Di portal Pertahanan Microsoft 365 di <https://security.microsoft.com> , masuk ke **Audit**. Atau, untuk langsung masuk ke **halaman Audit,** gunakan <https://security.microsoft.com/auditlogsearch> .

    **Catatan**: Jika Anda melihat pemberitahuan bahwa Anda perlu mengaktifkan fitur, lanjutkan dan aktifkan sekarang. Jika fitur tidak diaktifkan, hasil pencarian tidak akan dapat menarik data dari tanggal sebelumnya.

2. Pada tab **Pencarian** dari halaman **Audit,** konfigurasi pengaturan berikut ini:
   - **Rentang tanggal dan waktu**: Pilih rentang tanggal/waktu dalam **kotak** Mulai **dan** Akhir.
   - **Aktivitas**: Masukkan **Exchange kotak surat** lalu pilih nilai berikut:
     - **Pesan terhapus dari folder Item Dihapus**
     - **Memindahkan pesan ke folder Item Dihapus**

       Jika sudah selesai, klik di luar panel untuk meminimalkan **panel** Aktivitas.

   - **Pengguna**: Terima nilai default kosong untuk mengembalikan hasil bagi semua pengguna, atau masukkan satu atau beberapa pengguna.

3. Bila Anda sudah selesai, klik **Cari.** Aktivitas akan muncul di halaman **Pencarian audit baru.**

4. Pilih aktivitas dalam hasil untuk membuka flyout detail. Informasi tambahan tentang item yang dihapus, seperti baris subjek dan lokasi item saat item dihapus, ditampilkan di **bidang ItemDampakalah.**

   **Catatan**: Anda tidak dapat memulihkan item yang dihapus menggunakan fitur log audit. Untuk memulihkan item yang dihapus, lihat [Memulihkan pesan email yang dihapus Outlook di web](https://support.microsoft.com/office/recover-deleted-email-messages-in-outlook-on-the-web-a8ca78ac-4721-4066-95dd-571842e9fb11).

Untuk informasi selengkapnya, lihat [Mencari log audit untuk menyelidiki masalah dukungan umum.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
