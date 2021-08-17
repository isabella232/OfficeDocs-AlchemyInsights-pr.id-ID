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
ms.openlocfilehash: 14a5a18bc1422572db567c9533fefe5a7e0120afd64df4a64623038cc063ce93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058653"
---
# <a name="find-events-performed-on-inbox-rules"></a>Menemukan acara yang dilakukan pada aturan kotak masuk

Ketika aturan kotak masuk dibuat, diubah, atau dihapus, kejadian direkam dalam log audit. Berikut cara meninjaunya:

1. Masuk ke [Office 365 Pusat & Kepatuhan .](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Pilih Pencarian > Pencarian log audit.

    > [!NOTE]
    > Jika melihat pemberitahuan bahwa Anda perlu mengaktifkan pengauditan, lanjutkan dan aktifkan sekarang. Jika fitur ini tidak diaktifkan, hasil pencarian tidak akan dapat mengambil data dari tanggal sebelumnya.
1. Pilih bidang Aktivitas dan temukan Exchange kotak surat Anda, lalu pilih New-InboxRule Membuat aturan kotak masuk dari Outlook Web App. Jika sudah selesai, klik di luar panel untuk meminimalkan panel Aktivitas.
1. Tentukan rentang tanggal, lalu di bidang Pengguna, pilih nama pengguna untuk pengguna yang ingin Anda selidiki. Anda bisa memilih lebih dari satu pengguna dalam satu waktu.
1. Pilih Pencarian. Aktivitas muncul di bawah Hasil.
1. Untuk melihat detail, pilih aktivitas, lalu pilih Informasi Selengkapnya. Di bawah bagian Parameter Anda bisa melihat nama aturan, kumpulan ketentuan, dan tindakan yang akan diambil aturan.

Untuk mempelajari selengkapnya, lihat Mencari Office 365 log audit untuk memecahkan masalah skenario umum.