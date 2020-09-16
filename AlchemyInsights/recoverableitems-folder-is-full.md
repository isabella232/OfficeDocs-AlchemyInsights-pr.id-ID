---
title: folder 1336 RecoverableItems penuh
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
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741270"
---
# <a name="the-recoverable-items-folder-is-full"></a>Folder Item yang dapat dipulihkan penuh

Untuk kotak surat Exchange Online, batas penyimpanan default untuk folder Item yang dapat dipulihkan adalah 30 GB. Batas penyimpanan untuk folder Item yang dapat dipulihkan secara otomatis ditingkatkan ke 100 GB jika kotak surat ditempatkan pada penahanan litigasi, penangguhan eDiscovery, atau ditetapkan ke kebijakan penyimpanan.

Saat folder Item yang dapat dipulihkan mencapai batas penyimpanan, fungsionalitas kotak surat terpengaruh dengan cara berikut ini:

- Pengguna tidak dapat menghapus item dari kotak surat.

- Bantuan folder yang dikelola tidak dapat menghapus item berdasarkan pengaturan tag penyimpanan atau folder terkelola.

- Untuk kotak surat yang memiliki pemulihan satu item yang diaktifkan atau ditunda, proses proteksi halaman Salin pada penulisan tidak bisa mempertahankan versi item yang diedit oleh pengguna.

- Untuk kotak surat yang telah mengaktifkan pembuatan log audit kotak surat, tidak ada entri log audit kotak surat yang bisa disimpan dalam subfolder audit dalam folder Item yang dapat dipulihkan.

Untuk kotak surat yang tidak ditunda, admin dapat menggunakan `Search-Mailbox -SearchDumpsterOnly -DeleteContent` perintah di Exchange Online PowerShell untuk menghapus item di folder Item yang dapat dipulihkan. Untuk informasi selengkapnya, lihat topik berikut ini:

- [Mencari dan menghapus pesan](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Kotak surat pencarian](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Untuk kotak surat yang ditangguhkan, admin harus menghapus penangguhan sebelum mereka bisa menghapus item dari folder Item yang dapat dipulihkan. Untuk informasi selengkapnya, lihat [menghapus item dalam folder Item yang dapat dipulihkan dari kotak surat berbasis awan yang ditahan](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Untuk membantu mencegah folder Item yang dapat dipulihkan agar tidak penuh, admin bisa menambah batas penyimpanan folder Item yang dapat dipulihkan untuk kotak surat yang ditahan dan menyiapkan kebijakan penyimpanan kotak surat yang memindahkan item dari folder Item yang dapat dipulihkan ke kotak surat arsip pengguna. Lihat [menambah kuota item yang dipulihkan untuk kotak surat yang ditahan](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
