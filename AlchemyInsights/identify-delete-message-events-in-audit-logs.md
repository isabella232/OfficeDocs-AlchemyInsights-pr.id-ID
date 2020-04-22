---
title: Mengidentifikasi menghapus peristiwa pesan di log audit
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 797a4b1146862faf91d2b9e8d74feade90f71650
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716499"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Log audit untuk pesan email yang dihapus

Mulai Januari 2019, Microsoft telah mengaktifkan pengelogan audit kotak surat secara default. Jika tidak, untuk meninjau menghapus peristiwa pesan untuk pengguna tertentu, Anda harus secara manual mengaktifkan tindakan Hapus untuk audit. Jika pencatatan audit kotak pesan sudah diaktifkan untuk organisasi Anda atau pengguna tertentu, ikuti langkah di bawah.

1. Masuk ke [Microsoft 365 keamanan & Compliance Center](https://protection.office.com/)

2. Klik **Cari dan investigasi** , lalu pilih **pencarian log audit**.

3. Pilih rentang tanggal di kolom tanggal **mulai** dan **tanggal akhir** . Tentukan username untuk pengguna yang ingin Anda menyelidiki (pengguna yang dihapus item). Di bidang **aktivitas** , pilih **pesan yang dihapus dari folder Item dihapus** dan **Pindahkan pesan ke folder Item dihapus**.

4. Klik **Cari**.

Di hasil, pilih rekaman audit. Dalam Flyout rincian, klik **informasi lebih lanjut**. Informasi tambahan tentang item yang dihapus (misalnya, baris subjek dan lokasi item saat dihapus) ditampilkan di bidang **Affecteditems** . Properti **Clientinfostring** akan menunjukkan jika penghapusan terjadi di Outlook, Outlook di web (sebelumnya dikenal sebagai Outlook Web App), atau perangkat lainnya.

Untuk selengkapnya, lihat [menentukan siapa yang mengatur penerusan email untuk kotak pesan](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).

**Catatan**: Anda tidak dapat mengambil item yang dihapus menggunakan fitur log audit. Untuk mengambil pesan yang dihapus di Outlook di web, lihat [memulihkan item yang dihapus di Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
