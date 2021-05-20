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
ms.openlocfilehash: 563f76f624f428a46894268b478cf05eb757b497
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539827"
---
# <a name="missing-emails-in-quarantine"></a>Email yang hilang di karantina"

Administrator bisa [menampilkan, merilis, atau menghapus pesan ini.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Untuk membuka Pusat & Keamanan, masuk ke [https://protection.office.com](https://protection.office.com/) . Untuk membuka halaman Karantina secara langsung, masuk ke [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Anda bisa mencari dengan nilai berikut:  

- **ID Pesan**: Pengidentifikasi pesan secara global unik. Jika Anda memilih pesan dalam daftar, nilai  **ID Pesan**  muncul di panel  **flyout**  Detail yang muncul. Admin dapat menggunakan jejak [pesan untuk](/microsoft-365/security/office-365-security/message-trace-scc) menemukan pesan dan nilai ID Pesan terkait.
- **Alamat email** pengirim : Alamat email pengirim tunggal.
- **Alamat email** penerima: Alamat email penerima tunggal.
- **Subjek**: Gunakan seluruh subjek pesan. Pencarian tidak peka huruf besar/kecil.

Setelah Anda memasukkan kriteria pencarian, klik ![ Tombol Refresh ](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** untuk memfilter hasil.

Cmdlets yang Anda gunakan untuk menampilkan dan mengelola pesan dan file di karantina adalah:
- [Delete-QuarantineMessage](/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](/powershell/module/exchange/get-quarantinemessage)
- [Pratinjau-KarantinaPesan:](/powershell/module/exchange/preview-quarantinemessage)Perhatikan bahwa cmdlet ini hanya untuk pesan, bukan file malware dari Pertahanan Microsoft untuk Office 365 untuk SharePoint Online, OneDrive for Business, atau Teams.
- [Release-QuarantineMessage](/powershell/module/exchange/release-quarantinemessage)