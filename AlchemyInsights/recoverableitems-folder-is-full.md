---
title: 1336 RecoverableItems folder penuh
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1336
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 14d46980caf7dac90e73c34482a3aee34382fa1f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/23/2019
ms.locfileid: "32389086"
---
# <a name="the-recoverable-items-folder-is-full"></a>Folder item dapat dipulihkan ini penuh

Untuk kotak pesan Exchange Online pada Office 365, batas penyimpanan default untuk folder item dapat dipulihkan adalah 30 GB. Batas penyimpanan untuk folder item dapat dipulihkan secara otomatis meningkat menjadi 100 GB jika kotak pesan ditempatkan di penahanan litigasi, terus eDiscovery, atau ditetapkan ke kebijakan penyimpanan Office 365.

Ketika folder item dapat dipulihkan mencapai batas penyimpanan, fungsi kotak pesan dipengaruhi dengan cara berikut:

- Pengguna tidak dapat menghapus item dari kotak pesan.

- Bantuan Folder yang dikelola tidak dapat menghapus item yang didasarkan pada pengaturan folder terkelola atau tag penyimpanan.

- Untuk pesan yang memiliki pemulihan satu Item diaktifkan atau ditempatkan di penahanan, proses perlindungan salinan pada menulis halaman tidak mempertahankan versi item yang disunting oleh pengguna.

- Untuk pesan yang memiliki kotak pesan yang diaktifkan pendataan audit, entri log audit kotak pesan tidak dapat disimpan dalam audit subfolder dalam folder item dapat dipulihkan.

Untuk kotak pesan yang tidak ditahan, admin dapat menggunakan `Search-Mailbox -SearchDumpsterOnly -DeleteContent` perintah di Exchange Online PowerShell untuk menghapus item dalam folder item dapat dipulihkan. Untuk informasi selengkapnya, lihat topik berikut ini: 

- [Mencari dan menghapus pesan](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Untuk kotak pesan yang ditahan, admin perlu menghapus penahanan sebelum mereka dapat item yang dihapus dari folder item dapat dipulihkan. Untuk informasi lebih lanjut, lihat [menghapus item dalam folder kotak pesan berbasis Internet pada menampung item dapat dipulihkan](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Untuk membantu mencegah folder item dapat dipulihkan menjadi penuh, admin dapat meningkatkan batas penyimpanan item dapat dipulihkan folder untuk kotak pesan di pegang dan mengatur kotak pesan kebijakan penyimpanan yang memindahkan item dari folder item dapat dipulihkan ke arsip pengguna kotak pesan. Melihat [item yang dapat dipulihkan kuota untuk kotak pesan di terus meningkatkan](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
