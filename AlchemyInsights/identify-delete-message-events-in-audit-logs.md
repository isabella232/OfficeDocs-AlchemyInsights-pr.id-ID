---
title: Mengidentifikasi kejadian penghapusan pesan dalam log audit
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f68b623abd0efa990df71e5bf1ea1c9e7367ed691b1752f68c971e973922a63d
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/11/2021
ms.locfileid: "57868421"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Log audit untuk pesan email yang dihapus

Mulai Januari 2019, Microsoft akan mengaktifkan pembuatan log audit kotak surat secara default. Jika tidak, untuk meninjau kejadian penghapusan pesan bagi pengguna tertentu, Anda harus mengaktifkan tindakan penghapusan secara manual untuk pengauditan. Jika pembuatan log audit kotak surat sudah diaktifkan untuk organisasi Anda atau untuk pengguna tertentu, ikuti langkah-langkah di bawah ini.

1. Masuk ke Pusat [Microsoft 365 Kepatuhan](https://protection.office.com/)

2. Klik **Pencarian dan Investigasi,** lalu **pilih Pencarian Log Audit.**

3. Pilih rentang tanggal di bidang **Tanggal mulai** **dan Tanggal** selesai. Tentukan nama pengguna untuk pengguna yang ingin Anda selidiki (pengguna yang menghapus item). Di bidang **Aktivitas,** pilih **Pesan terhapus dari folder Item Dihapus** dan Pesan yang **dipindahkan ke folder Item Dihapus.**

4. Klik **Cari.**

Dalam hasil, pilih catatan audit. Di flyout detail, klik **Informasi Selengkapnya.** Informasi tambahan tentang item yang dihapus (misalnya, baris subjek dan lokasi item saat item dihapus) ditampilkan di bidang ItemDampakalah.  Properti **ClientInfoString** akan memperlihatkan jika penghapusan terjadi di Outlook, Outlook di web (sebelumnya dikenal sebagai Outlook Web App), atau perangkat lainnya.

Untuk informasi selengkapnya, [lihat Menentukan siapa yang menyiapkan penerusan email untuk kotak surat](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**Catatan**: Anda tidak dapat mengambil item yang dihapus menggunakan fitur log audit. Untuk mengambil pesan yang dihapus di Outlook di web, lihat [Memulihkan item yang dihapus Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
