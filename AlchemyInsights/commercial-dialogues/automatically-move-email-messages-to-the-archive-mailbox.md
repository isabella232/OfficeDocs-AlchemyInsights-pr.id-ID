---
title: Memindahkan pesan email secara otomatis ke kotak surat Arsip
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746044"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>Memindahkan pesan email secara otomatis ke kotak surat Arsip

Berikut ini cara menyiapkan kebijakan untuk secara otomatis memindahkan email lama pengguna ke kotak surat Arsip:

1. Masuk ke [](https://go.microsoft.com/fwlink/p/?linkid=2077143)  >  **Arsip tata kelola data** kepatuhan & keamanan  >   untuk memverifikasi kotak surat Arsip telah diaktifkan untuk pengguna. Jika belum, klik **Aktifkan** lalu **ya** dalam kotak peringatan.
2. Masuk ke [**Pusat admin Exchange > manajemen kepatuhan > tag penyimpanan**](https://go.microsoft.com/fwlink/?linkid=2059104).
3. Pilih ikon + lalu pilih **Terapkan secara otomatis ke seluruh kotak surat**.
4. Tetapkan nama ke tag penyimpanan, dan pilih **Pindahkan ke arsip**. Untuk periode penyimpanan, masukkan waktu yang Anda inginkan, seperti 90 hari. Klik **Simpan**.
5. Sekarang Buat kebijakan penyimpanan: Pilih **kebijakan penyimpanan**, pilih ikon untuk menambahkan kebijakan baru.
6. Tetapkan nama ke kebijakan penyimpanan, lalu klik dan gulir untuk menemukan dan menambahkan tag penyimpanan yang baru Anda buat. Klik **Simpan**.
7. Terakhir, Terapkan kebijakan penyimpanan ke kotak surat pengguna: masih di pusat admin Exchange, masuk ke   >  **kotak surat** Penerima. Pilih Semua pengguna yang ingin Anda Terapkan kebijakannya, lalu pilih **Edit** (ikon pensil).
8. Dalam kotak dialog, klik **fitur kotak surat**. Di bawah **kebijakan penyimpanan**, Terapkan kebijakan yang baru anda buat > **Simpan**.
9. Untuk instruksi tentang penerapan kebijakan kepada semua pengguna, lihat [menerapkan kebijakan penyimpanan ke kotak surat](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).
