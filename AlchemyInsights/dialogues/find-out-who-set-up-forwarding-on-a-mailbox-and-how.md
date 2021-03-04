---
title: Mencari tahu siapa yang menyetel penerusan pada kotak surat, dan caranya
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
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429616"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Mencari tahu siapa yang menyetel penerusan pada kotak surat, dan caranya

Jika penerusan eksternal diatur di kotak surat, aktivitas diaudit sebagai bagian dari cmdlet Set-Mailbox. Berikut cara menemukan aktivitas dalam log audit:

1. Masuk ke [pusat kepatuhan & keamanan Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. Pilih **Cari pencarian** >  **log audit**.
    > [!NOTE]
    > Jika Anda melihat pemberitahuan bahwa Anda perlu mengaktifkan pengauditan, Lanjutkan dan Aktifkan sekarang. Jika fitur ini tidak diaktifkan, hasil pencarian tidak akan dapat menarik data dari tanggal sebelumnya.
1. Pastikan bidang **aktivitas** diatur untuk **memperlihatkan hasil untuk semua aktivitas** (default). Menentukan rentang tanggal. Anda tidak perlu menentukan nama pengguna.
1. Pilih **pencarian**. Aktivitas muncul di bawah **hasil**.
1. Pilih **filter hasil**, lalu masukkan **set-kotak surat** di bidang filter **aktivitas** . Ini mengembalikan semua aktivitas **kumpulan-kotak surat** .
1. Untuk menampilkan detail, pilih aktivitas, lalu pilih **informasi lainnya**. Di bawah **parameter** Anda dapat melihat alamat email penerusan yang diatur di kotak surat. **Userid** mewakili pengguna yang menyetel penerusan eksternal pada kotak surat.
Untuk mempelajari selengkapnya, lihat [mencari log audit Office 365 untuk memecahkan masalah skenario umum](https://go.microsoft.com/fwlink/?linkid=2103944).