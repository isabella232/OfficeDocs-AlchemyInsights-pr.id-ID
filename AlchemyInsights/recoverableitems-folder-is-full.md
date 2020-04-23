---
title: 1336 RecoverableItems folder penuh
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: fb10b792981040bdcf4661b8aff30733c2438212
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720255"
---
# <a name="the-recoverable-items-folder-is-full"></a>Folder item dapat dipulihkan penuh

Untuk kotak surat Exchange Online, batas penyimpanan default untuk folder item dapat dipulihkan adalah 30 GB. Batas penyimpanan untuk folder item dapat dipulihkan akan secara otomatis ditingkatkan ke 100 GB jika kotak pesan ditempatkan di penahanan litigasi, pembekuan eDiscovery, atau ditetapkan ke kebijakan penyimpanan.

Bila folder item dapat dipulihkan mencapai batas penyimpanan, fungsi kotak pesan akan terpengaruh dengan cara berikut:

- Pengguna tidak dapat menghapus item dari kotak surat.

- Bantuan folder yang dikelola tidak dapat menghapus item berdasarkan Tag penyimpanan atau pengaturan Folder Terkelola.

- Untuk kotak pesan yang memiliki pemulihan satu item diaktifkan atau ditempatkan di tahan, proses perlindungan halaman salinan-on-Write tidak dapat mempertahankan versi item yang diedit oleh pengguna.

- Untuk kotak pesan yang memiliki pencatatan audit kotak pesan aktif, tidak ada entri log audit kotak pesan yang dapat disimpan di subfolder audit dalam folder Item bisa dipulihkan.

Untuk kotak pesan yang tidak di tahan, admin dapat menggunakan `Search-Mailbox -SearchDumpsterOnly -DeleteContent` perintah di Exchange Online PowerShell untuk menghapus item dalam folder item dapat dipulihkan. Untuk informasi selengkapnya, lihat topik berikut ini:

- [Mencari dan menghapus pesan](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [Kotak pesan penelusuran](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Untuk kotak pesan yang sedang di tahan, admin harus menghapus terus sebelum mereka dapat menghapus item dari folder Item bisa dipulihkan. Untuk selengkapnya, lihat [menghapus item di folder item dapat dipulihkan dari kotak pesan berbasis Internet yang akan ditahan](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Untuk membantu mencegah folder item dapat dipulihkan menjadi penuh, admin dapat meningkatkan batas penyimpanan folder item dapat dipulihkan untuk kotak pesan yang ditangguhkan dan mengatur kebijakan retensi kotak pesan yang memindahkan item dari folder item dapat dipulihkan ke kotak pesan arsip pengguna. Lihat [meningkatkan kuota item dapat dipulihkan untuk kotak pesan yang akan ditahan](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
