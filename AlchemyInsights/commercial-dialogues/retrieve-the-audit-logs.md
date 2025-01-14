---
title: Mengambil log audit
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
ms.openlocfilehash: 88d28898923c1381c001c15445da90901b7e8761
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320446"
---
# <a name="retrieve-the-audit-logs"></a>Mengambil log audit

Saat pertama kali Anda membuka log audit, log audit akan kosong. Anda harus melakukan pencarian untuk melihat apa yang ada di sana. Berikut cara melakukan pencarian umum untuk semua aktivitas:

1. Lakukan salah satu tindakan berikut ini:
   - Pada bagian pusat kepatuhan Microsoft 365 <https://compliance.microsoft.com> , masuk ke **Audit** \> **Solusi**. Atau, untuk langsung masuk ke **halaman Audit,** gunakan <https://compliance.microsoft.com/auditlogsearch> .
   - Di portal Pertahanan Microsoft 365 di <https://security.microsoft.com> , masuk ke **Audit**. Atau, untuk langsung masuk ke **halaman Audit,** gunakan <https://security.microsoft.com/auditlogsearch> .

2. Pada tab **Pencarian** dari halaman **Audit,** konfigurasi pengaturan berikut ini:
   - **Rentang tanggal dan waktu**: Pilih rentang tanggal/waktu dalam **kotak** Mulai **dan** Akhir.
   - **Aktivitas**: Verifikasi **bahwa Perlihatkan hasil untuk semua** aktivitas dipilih.
   - **Pengguna**: Terima nilai default kosong untuk mengembalikan hasil bagi semua pengguna, atau masukkan satu atau beberapa pengguna.

3. Bila Anda sudah selesai, klik **Cari.** Aktivitas akan muncul di halaman **Pencarian audit baru.**

4. Pilih aktivitas dalam hasil untuk membuka flyout detail. Anda akan melihat informasi selengkapnya seperti Klien, Pengguna yang melakukan tindakan, dll.

Untuk mempelajari selengkapnya, lihat [Mencari log audit untuk menyelidiki masalah dukungan umum.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
