---
title: Memindahkan pesan email secara otomatis ke kotak surat arsip
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
ms.openlocfilehash: 57dbfd116bbae227f2288ce23edeaaa833fadf54ca3b10b95c49512758542e32
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059229"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>Memindahkan pesan email secara otomatis ke kotak surat arsip

Berikut cara menyiapkan kebijakan untuk memindahkan email lama pengguna ke kotak surat arsip secara otomatis:

1. Masuk ke [**Arsip & tata**](https://go.microsoft.com/fwlink/p/?linkid=2077143)kelola  >  **Data**  >  **Kepatuhan** untuk memverifikasi bahwa kotak surat arsip telah diaktifkan untuk pengguna. Jika belum muncul, klik Aktifkan **lalu** **Ya** dalam kotak peringatan.
2. Masuk ke [**Exchange admin > manajemen kepatuhan > tag penyimpanan**](https://go.microsoft.com/fwlink/?linkid=2059104).
3. Pilih ikon + lalu pilih terapkan **secara otomatis ke seluruh kotak surat**.
4. Tetapkan nama untuk tag penyimpanan, lalu pilih **Pindahkan ke Arsip**. Untuk periode penyimpanan, masukkan waktu yang Anda inginkan, seperti 90 hari. Klik **Simpan**.
5. Sekarang buat kebijakan penyimpanan: pilih **kebijakan penyimpanan**, pilih ikon untuk menambahkan kebijakan baru.
6. Tetapkan nama kebijakan penyimpanan, lalu klik dan gulir untuk menemukan dan menambahkan tag penyimpanan yang baru Anda buat. Klik **Simpan**.
7. Terakhir, terapkan kebijakan penyimpanan ke kotak surat pengguna: masih dalam pusat admin Exchange, masuk ke **kotak surat**  >  **penerima**. Pilih semua pengguna yang ingin Anda terapkan kebijakannya, lalu pilih **Edit** (ikon pensil).
8. Dalam kotak dialog, klik fitur **kotak surat**. Di **bawah Kebijakan** penyimpanan , terapkan kebijakan yang baru Anda buat > **Simpan**.
9. Untuk instruksi menerapkan kebijakan ke semua pengguna, lihat [Menerapkan kebijakan penyimpanan ke kotak surat](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).
