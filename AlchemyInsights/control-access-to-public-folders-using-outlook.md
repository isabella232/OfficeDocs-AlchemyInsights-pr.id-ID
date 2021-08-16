---
title: Kontrol akses ke folder publik menggunakan Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 1386b97f804e63455094abf64b9d9e2541d57dafa36535813b0d7689e0ce2966
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54032561"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Kontrol akses ke folder publik menggunakan Outlook

Untuk mengontrol pengguna mana yang dapat mengakses folder publik menggunakan Outlook:

1. Gunakan `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: Izinkan pengguna mengakses folder publik di Outlook  
$false: Cegah pengguna mengakses folder publik di Outlook. Ini adalah nilai default.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Catatan: Prosedur ini hanya dapat mengontrol koneksi dengan Outlook versi desktop untuk klien Windows. Pengguna dapat terus mengakses folder publik menggunakan OWA atau Outlook untuk Mac.

Untuk informasi selengkapnya, lihat [Koneksi Terkontrol ke Folder Publik di Outlook](https://aka.ms/controlpf).
