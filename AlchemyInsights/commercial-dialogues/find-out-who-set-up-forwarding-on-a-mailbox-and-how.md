---
title: Cari tahu siapa yang menyiapkan penerusan di kotak surat, dan caranya
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
ms.openlocfilehash: 6243e787bb6b51f26cf22782d9ec80f946430b864f53de7ea626b7166a674d2c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988206"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Cari tahu siapa yang menyiapkan penerusan di kotak surat, dan caranya

Jika penerusan eksternal diatur di kotak surat, aktivitas akan diaudit sebagai bagian dari cmdlet Set-Mailbox cmdlet. Berikut cara menemukan aktivitas dalam log audit:

1. Masuk ke [Office 365 Pusat & Kepatuhan .](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Pilih **Pencarian** >  **pencarian log Audit**.
    > [!NOTE]
    > Jika melihat pemberitahuan bahwa Anda perlu mengaktifkan pengauditan, lanjutkan dan aktifkan sekarang. Jika fitur ini tidak diaktifkan, hasil pencarian tidak akan dapat mengambil data dari tanggal sebelumnya.
1. Pastikan bidang **Aktivitas** diatur ke **Perlihatkan hasil untuk semua aktivitas** (default). Tentukan rentang tanggal. Anda tidak perlu menentukan nama pengguna.
1. Pilih **Pencarian.** Aktivitas muncul di bawah **Hasil.**
1. Pilih **Filter Hasil**, lalu masukkan **Set-mailbox** dalam **bidang** filter Aktivitas. Ini akan mengembalikan semua **aktivitas Set-Mailbox.**
1. Untuk melihat detail, pilih aktivitas, lalu pilih **Informasi Selengkapnya**. Di **bawah** Parameter, Anda dapat melihat alamat email penerusan yang diatur di kotak surat. **UserID** mewakili pengguna yang menyiapkan penerusan eksternal pada kotak surat.
Untuk mempelajari selengkapnya, lihat [Mencari Office 365 log audit untuk memecahkan masalah skenario umum](https://go.microsoft.com/fwlink/?linkid=2103944).