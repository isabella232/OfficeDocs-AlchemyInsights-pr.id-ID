---
title: Menemukan alamat IP di log audit
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
ms.openlocfilehash: 5b58803719df700290f495cb2d2d6742f072420a2a1d393534ca165bb5a14fbb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54017135"
---
# <a name="find-the-ip-address-in-audit-log"></a>Menemukan alamat IP di log audit

1. Alamat IP yang berkaitan dengan aktivitas yang dilakukan oleh pengguna atau administrator diperlihatkan dalam log audit. Informasi klien juga dicatat. Berikut cara mengidentifikasi alamat IP tersebut:

1. Masuk ke [Office 365 Pusat & Kepatuhan .](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Pilih **Pencarian**  >  **[pencarian log Audit](https://go.microsoft.com/fwlink/?linkid=2103759)**.
    > [!NOTE]
    > Jika melihat pemberitahuan bahwa Anda perlu mengaktifkan pengauditan, lanjutkan dan aktifkan sekarang. Jika fitur ini tidak diaktifkan, hasil pencarian tidak akan dapat mengambil data dari tanggal sebelumnya.
1. Jika Anda tertarik pada aktivitas tertentu, pilih aktivitas tersebut dari **daftar** Aktivitas; jika tidak, secara default, semua aktivitas akan dikembalikan untuk pengguna yang dipilih. Perhatikan bahwa aktivitas tertentu mungkin tidak tersedia untuk dipilih **dari** menu Aktivitas; namun, item audit tersebut akan dikembalikan jika **Perlihatkan hasil untuk semua aktivitas** dipilih (pengaturan default).
1. Tentukan rentang tanggal, dan di bidang **Pengguna,** pilih nama pengguna untuk pengguna yang ingin Anda selidiki.
1. Pilih **Pencarian.** Aktivitas muncul di bawah **Hasil.** Anda dapat melihat alamat IP untuk setiap aktivitas.
1. Untuk melihat detail, pilih aktivitas, lalu pilih **Informasi Selengkapnya**.

Untuk mempelajari selengkapnya, lihat Mencari [Office 365 log audit untuk memecahkan masalah skenario umum](https://go.microsoft.com/fwlink/?linkid=2103944).