---
title: Tidak bisa mengakses folder publik
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
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819515"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook tidak bisa tersambung ke folder publik

Jika akses folder publik tidak berfungsi untuk beberapa pengguna, cobalah hal berikut:

Sambungkan ke EXO PowerShell dan konfigurasi parameter DefaultPublicFolderMailbox pada akun pengguna yang bermasalah agar sesuai dengan parameter pada akun pengguna yang berfungsi.

Contoh:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Tunggu setidaknya satu jam agar perubahan bisa diterapkan.

Jika masalah tetap terjadi, ikuti prosedur [ini untuk](https://aka.ms/pfcte) memecahkan masalah akses folder publik menggunakan Outlook.
 
**Untuk mengontrol pengguna mana yang bisa mengakses folder publik menggunakan Outlook:**

1.  Gunakan Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true atau $false  
      
    $true: Memungkinkan pengguna mengakses folder publik di Outlook  
      
    $false: Mencegah akses pengguna ke folder publik di Outlook. Ini adalah nilai default.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Catatan** Prosedur ini hanya bisa mengontrol koneksi dengan desktop Outlook untuk klien Windows. Pengguna bisa terus mengakses folder publik menggunakan OWA atau Outlook untuk Mac.
 
Untuk informasi selengkapnya, [lihat Mengumumkan Dukungan untuk Koneksi Terkontrol ke Folder Publik di Outlook](https://aka.ms/controlpf).