---
title: Mengidentifikasi menghapus acara pesan dalam log audit
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
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696516"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Log audit untuk pesan email yang dihapus

Mulai Januari 2019, Microsoft mengaktifkan pembuatan log audit kotak surat secara default. Jika tidak, untuk meninjau menghapus acara pesan untuk pengguna tertentu, Anda perlu mengaktifkan tindakan penghapusan untuk pengauditan secara manual. Jika pembuatan log audit kotak surat sudah diaktifkan untuk organisasi Anda atau pengguna tertentu, ikuti langkah-langkah di bawah ini.

1. Masuk ke [pusat kepatuhan & keamanan Microsoft 365](https://protection.office.com/)

2. Klik **pencarian dan investigasi** dan pilih **pencarian log audit**.

3. Pilih rentang tanggal di bidang tanggal **mulai** dan **tanggal berakhir** . Tentukan nama pengguna untuk pengguna yang ingin Anda selidiki (pengguna yang menghapus item). Di bidang **aktivitas** , pilih **pesan yang dihapus dari folder Item terhapus** dan **Pindahkan pesan ke folder Item terhapus**.

4. Klik **Cari**.

Dalam hasil, pilih catatan audit. Dalam Flyout detail, klik **informasi selengkapnya**. Informasi tambahan tentang item terhapus (misalnya, baris subjek dan lokasi item saat dihapus) ditampilkan di bidang **Affecteditems** . Properti **Clientinfostring** akan ditampilkan jika penghapusan terjadi di Outlook, Outlook di web (sebelumnya dikenal sebagai Outlook Web App), atau perangkat lain.

Untuk informasi selengkapnya, lihat [menentukan siapa yang menyetel penerusan email untuk kotak surat](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**Catatan**: Anda tidak bisa mengambil item terhapus menggunakan fitur log audit. Untuk mengambil pesan yang dihapus di Outlook di web, lihat [memulihkan item terhapus di Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
