---
title: Membaca log audit untuk acara yang dihapus
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
ms.openlocfilehash: 9739fb1eb8e4f5adf81cd699c851a51176f0429e
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482264"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>Membaca log audit untuk acara yang dihapus

Berikut ini cara melakukan ini:

1. Masuk ke [pusat kepatuhan & keamanan Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. Pilih **Cari pencarian**  >  [**log audit**](https://go.microsoft.com/fwlink/?linkid=2103759).
    > [!NOTE]
    > Jika Anda melihat pemberitahuan bahwa Anda perlu mengaktifkan fitur tersebut, Lanjutkan dan Aktifkan sekarang. Jika fitur tidak diaktifkan, hasil pencarian tidak akan dapat menarik data dari tanggal sebelumnya.
1. Pilih **aktivitas**, lalu temukan **aktivitas kotak surat Exchange**. Pilih opsi Hapus **pesan dari folder Item terhapus** dan **Pindahkan pesan ke folder Item terhapus** . Bila sudah selesai, klik di luar panel untuk meminimalkan panel **aktivitas** .
1. Tentukan rentang tanggal, lalu di kotak **pengguna** , pilih nama pengguna yang ingin Anda selidiki. Anda dapat memilih lebih dari satu pengguna dalam satu waktu.
1. Pilih **pencarian**. Aktivitas muncul di bawah **hasil**.
1. Untuk menampilkan detail, pilih aktivitas, lalu pilih **informasi lainnya**. Informasi tambahan tentang item terhapus, seperti baris subjek dan lokasi item saat dihapus, ditampilkan di bidang **Affecteditems** .
    > [!NOTE]
    > Anda tidak bisa memulihkan item terhapus menggunakan fitur log audit. Untuk memulihkan item yang dihapus, lihat [memulihkan item atau email terhapus di Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).

Untuk mempelajari selengkapnya, lihat [mencari log audit Office 365 untuk memecahkan masalah skenario umum](https://go.microsoft.com/fwlink/?linkid=2103944).
