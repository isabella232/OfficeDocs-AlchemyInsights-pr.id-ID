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
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816743"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Kontrol akses ke folder publik menggunakan Outlook

Untuk mengontrol pengguna mana yang dapat mengakses folder publik menggunakan Outlook:

1. Gunakan `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: Izinkan pengguna mengakses folder publik di Outlook  
$false: Cegah pengguna mengakses folder publik di Outlook. Ini adalah nilai default.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Catatan: Prosedur ini hanya dapat mengontrol koneksi dengan Outlook versi desktop untuk klien Windows. Pengguna dapat terus mengakses folder publik menggunakan OWA atau Outlook untuk Mac.

Untuk informasi selengkapnya, lihat [Koneksi Terkontrol ke Folder Publik di Outlook](https://aka.ms/controlpf).
