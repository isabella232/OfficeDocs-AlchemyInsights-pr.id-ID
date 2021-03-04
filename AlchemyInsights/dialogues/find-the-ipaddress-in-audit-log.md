---
title: Menemukan alamat IP dalam log audit
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
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429508"
---
# <a name="find-the-ip-address-in-audit-log"></a>Menemukan alamat IP dalam log audit

1. Alamat IP yang terkait dengan aktivitas yang dilakukan oleh pengguna atau administrator diperlihatkan dalam log audit. Informasi klien juga dicatat. Berikut cara mengidentifikasi alamat IP:

1. Masuk ke [pusat kepatuhan & keamanan Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. Pilih **Cari pencarian**  >  **[log audit](https://go.microsoft.com/fwlink/?linkid=2103759)**.
    > [!NOTE]
    > Jika Anda melihat pemberitahuan bahwa Anda perlu mengaktifkan pengauditan, Lanjutkan dan Aktifkan sekarang. Jika fitur ini tidak diaktifkan, hasil pencarian tidak akan dapat menarik data dari tanggal sebelumnya.
1. Jika Anda tertarik dengan aktivitas tertentu, pilih dari daftar **aktivitas** ; Jika tidak, secara default, semua aktivitas akan dikembalikan untuk pengguna yang dipilih. Perhatikan bahwa aktivitas tertentu mungkin tidak tersedia untuk pilihan dari menu **aktivitas** ; Namun, item audit tersebut akan dikembalikan jika **memperlihatkan hasil untuk semua aktivitas** yang dipilih (pengaturan default).
1. Tentukan rentang tanggal, dan di bidang **pengguna** , pilih nama pengguna yang ingin Anda selidiki.
1. Pilih **pencarian**. Aktivitas muncul di bawah **hasil**. Anda dapat melihat alamat IP untuk setiap aktivitas.
1. Untuk menampilkan detail, pilih aktivitas, lalu pilih **informasi lainnya**.

Untuk mempelajari selengkapnya, lihat mencari [log audit Office 365 untuk memecahkan masalah skenario umum](https://go.microsoft.com/fwlink/?linkid=2103944).