---
title: Email yang hilang di karantina
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831737"
---
# <a name="missing-emails-in-quarantine"></a>Email yang hilang di karantina"

Administrator bisa [menampilkan, merilis, atau menghapus pesan ini.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Untuk membuka Pusat & Keamanan, masuk ke [https://protection.office.com](https://protection.office.com/) . Untuk membuka halaman Karantina secara langsung, masuk ke [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Anda bisa mencari dengan nilai berikut:  

- **ID Pesan**: Pengidentifikasi pesan secara global unik. Jika Anda memilih pesan dalam daftar, nilai  **ID Pesan**  muncul di panel  **flyout**  Detail yang muncul. Admin dapat menggunakan jejak [pesan untuk](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) menemukan pesan dan nilai ID Pesan terkait.
- **Alamat email** pengirim : Alamat email pengirim tunggal.
- **Alamat email** penerima: Alamat email penerima tunggal.
- **Subjek**: Gunakan seluruh subjek pesan. Pencarian tidak peka huruf besar/kecil.

Setelah Anda memasukkan kriteria pencarian, klik ![ Tombol Refresh ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** untuk memfilter hasil.  

Cmdlets yang Anda gunakan untuk menampilkan dan mengelola pesan dan file di karantina adalah:
- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Pratinjau-KarantinaPesan:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)Perhatikan bahwa cmdlet ini hanya untuk pesan, bukan file malware dari ATP untuk SharePoint Online, OneDrive for Business, atau Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)