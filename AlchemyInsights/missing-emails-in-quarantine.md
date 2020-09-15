---
title: Email yang hilang dalam karantina
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673717"
---
# <a name="missing-emails-in-quarantine"></a>Email yang hilang dalam karantina "

Administrator bisa [menampilkan, melepaskan, atau menghapus pesan ini.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Untuk membuka pusat kepatuhan & keamanan, masuk ke [https://protection.office.com](https://protection.office.com/) . Untuk membuka halaman karantina secara langsung, masuk ke [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Anda dapat mencari menurut nilai berikut ini:  

- **Id pesan**: pengidentifikasi pesan yang unik secara global. Jika Anda memilih pesan dalam daftar, nilai  **id pesan**  muncul di panel  **rincian**  Flyout yang muncul. Admin dapat menggunakan [pelacakan pesan](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) untuk menemukan pesan dan nilai id pesan terkait.
- **Alamat email pengirim**: alamat email pengirim tunggal.
- **Alamat email penerima**: alamat email penerima tunggal.
- **Subjek**: Gunakan seluruh subjek pesan. Pencarian tidak peka huruf besar-kecil.

Setelah memasukkan kriteria pencarian, klik Refresh tombol refresh ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** untuk memfilter hasil.  

Cmdlet yang Anda gunakan untuk menampilkan dan mengelola pesan dan file dalam karantina adalah:
- [Hapus-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Ekspor-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Dapatkan-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Pratinjau-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Perhatikan bahwa cmdlet ini hanya untuk pesan, bukan file MALWARE dari ATP untuk SharePoint online, OneDrive for Business, atau teams.
- [Rilis-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)