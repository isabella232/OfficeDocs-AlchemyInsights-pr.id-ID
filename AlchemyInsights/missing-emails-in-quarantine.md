---
title: Email tidak ada di karantina
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569232"
---
# <a name="missing-emails-in-quarantine"></a>Email tidak ada di karantina "

Administrator dapat [melihat, melepaskan, atau menghapus pesan ini.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Untuk membuka pusat kepatuhan & keamanan, kunjungi [https://protection.office.com](https://protection.office.com/) . Untuk membuka halaman karantina secara langsung, kunjungi [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Anda dapat mencari dengan nilai berikut:  

- **Id pesan**: pengidentifikasi unik global pesan. Jika Anda memilih pesan dalam daftar, nilai **id pesan** akan muncul di panel Flyout **rincian** yang muncul. Admin dapat menggunakan [pelacakan pesan](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) untuk menemukan pesan dan nilai id pesan yang sesuai.
- **Alamat email pengirim**: alamat email pengirim tunggal.
- **Alamat email penerima**: alamat email penerima tunggal.
- **Subjek**: Gunakan seluruh subjek pesan. Pencarian tidak peka terhadap huruf besar-kecil.

Setelah Anda memasukkan kriteria pencarian, klik Refresh ![ tombol ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **refresh** untuk menyaring hasil.  

Cmdlet yang Anda gunakan untuk melihat dan mengelola pesan dan file dalam karantina adalah:
- [Hapus-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Ekspor-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Pratinjau-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Perhatikan bahwa cmdlet ini hanya untuk pesan, bukan berkas MALWARE dari ATP untuk SharePoint online, OneDrive untuk bisnis, atau tim.
- [Rilis-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)