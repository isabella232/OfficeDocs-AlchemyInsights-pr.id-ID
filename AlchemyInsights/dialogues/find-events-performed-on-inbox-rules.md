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
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429628"
---
# <a name="find-events-performed-on-inbox-rules"></a>Menemukan acara yang dilakukan pada aturan kotak masuk

Saat aturan kotak masuk dibuat, diubah, atau dihapus, kejadian dicatat dalam log audit. Berikut ini cara untuk meninjau mereka:

1. Masuk ke [pusat kepatuhan & keamanan Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. Pilih pencarian > pencarian log audit.

    > [!NOTE]
    > Jika Anda melihat pemberitahuan bahwa Anda perlu mengaktifkan pengauditan, Lanjutkan dan Aktifkan sekarang. Jika fitur ini tidak diaktifkan, hasil pencarian tidak akan dapat menarik data dari tanggal sebelumnya.
1. Pilih bidang aktivitas dan temukan aktivitas kotak surat Exchange, lalu pilih New-InboxRule Buat aturan kotak masuk dari Outlook Web App. Bila sudah selesai, klik di luar panel untuk meminimalkan panel aktivitas.
1. Tentukan rentang tanggal, lalu di bidang pengguna, pilih nama pengguna yang ingin Anda selidiki. Anda dapat memilih lebih dari satu pengguna dalam satu waktu.
1. Pilih pencarian. Aktivitas muncul di bawah hasil.
1. Untuk menampilkan detail, pilih aktivitas, lalu pilih informasi lainnya. Di bawah bagian parameter, Anda bisa melihat nama aturan, ketentuan yang ditetapkan, dan tindakan yang akan diambil oleh aturan tersebut.

Untuk mempelajari selengkapnya, lihat mencari log audit Office 365 untuk memecahkan masalah skenario umum.