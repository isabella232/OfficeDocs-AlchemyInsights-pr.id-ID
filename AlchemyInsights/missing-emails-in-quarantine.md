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
ms.openlocfilehash: c77da6716c0755d6ed4911f490e000bd74d08f92
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329665"
---
# <a name="missing-emails-in-quarantine"></a>Email yang hilang di karantina

Administrator bisa [menampilkan, merilis, atau menghapus pesan ini](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Di portal Pertahanan Microsoft 365 di <https://security.microsoft.com> , masuk ke **Tinjau** \> **Karantina**. Atau, untuk langsung masuk ke halaman **Karantina,** gunakan <https://security.microsoft.com/quarantine> .  

Untuk informasi selengkapnya tentang nilai pencarian/filter yang dapat Anda gunakan, lihat Mengelola pesan dan file yang [dikarantina sebagai admin di EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files).

Cmdlet yang Anda gunakan untuk menampilkan dan mengelola pesan dan file di karantina adalah:

- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Pratinjau-KarantinaPesan:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)Perhatikan bahwa cmdlet ini hanya untuk pesan, bukan file dari Brankas Lampiran untuk SharePoint, OneDrive, atau Microsoft Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
