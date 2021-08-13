---
title: 1336 folder RecoverableItems sudah penuh
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
ms.openlocfilehash: 5c8d53ceabf2428f3d6d765040f1b789b6bbeda04a22dd7fde0d2d728fd17d93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061759"
---
# <a name="the-recoverable-items-folder-is-full"></a>Folder Item yang Dapat Dipulihkan sudah penuh

Untuk Exchange Online kotak surat, batas penyimpanan default untuk folder Item yang Dapat Dipulihkan adalah 30 GB. Batas penyimpanan folder Item yang Dapat Dipulihkan secara otomatis ditingkatkan menjadi 100 GB jika kotak surat ditempatkan dalam Penyimpanan Litigasi, penyimpanan eDiscovery, atau ditetapkan ke kebijakan penyimpanan.

Saat folder Item yang Dapat Dipulihkan mencapai batas penyimpanan, fungsionalitas kotak surat akan terpengaruh dengan cara-cara berikut:

- Pengguna tidak dapat menghapus item dari kotak surat.

- Asisten Folder Terkelola tidak bisa menghapus item berdasarkan tag penyimpanan atau pengaturan folder terkelola.

- Untuk kotak surat dengan Pemulihan Item Tunggal yang diaktifkan atau ditahan, proses perlindungan halaman salin-saat-tulis tidak dapat mempertahankan versi item yang diedit oleh pengguna.

- Untuk kotak surat yang mengaktifkan pembuatan log audit kotak surat, tidak ada entri log audit kotak surat yang dapat disimpan di subfolder Audit dalam folder Item yang Dapat Dipulihkan.

Untuk kotak surat yang tidak ditahan, admin dapat menggunakan perintah di PowerShell Exchange Online menghapus item dalam `Search-Mailbox -SearchDumpsterOnly -DeleteContent` folder Item yang Dapat Dipulihkan. Untuk informasi selengkapnya, lihat topik berikut ini:

- [Mencari dan menghapus pesan](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Untuk kotak surat yang sedang ditahan, admin harus menghapus penahanan tersebut sebelum dapat menghapus item dari folder Item yang Dapat Dipulihkan. Untuk informasi selengkapnya, [lihat Menghapus item dalam folder Item yang Dapat Dipulihkan dari kotak surat berbasis awan saat sedang menahan](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Untuk membantu mencegah folder Item yang Dapat Dipulihkan menjadi penuh, admin dapat meningkatkan batas penyimpanan folder Item yang Dapat Dipulihkan untuk kotak surat yang ditahan dan menetapkan kebijakan penyimpanan kotak surat yang memindahkan item dari folder Item Dapat Dipulihkan ke kotak surat arsip pengguna. Lihat [Menambah kuota Item yang Dapat Dipulihkan untuk kotak surat saat kotak surat ditahan.](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold)
