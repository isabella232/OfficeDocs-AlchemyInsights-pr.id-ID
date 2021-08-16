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
ms.openlocfilehash: f129da8731877aa00fd9b1dcf20905d353a4895303390ce7ff5642a8ff3ccbc2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53996633"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook tidak bisa tersambung ke folder publik

Jika akses folder publik tidak berfungsi untuk beberapa pengguna, cobalah hal berikut:

Koneksi ke EXO PowerShell dan konfigurasi parameter DefaultPublicFolderMailbox pada akun pengguna yang bermasalah agar sesuai dengan parameter pada akun pengguna yang berfungsi.

Contoh:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Tunggu setidaknya satu jam agar perubahan bisa diterapkan.

Jika masalah tetap terjadi, ikuti prosedur [ini untuk](https://aka.ms/pfcte) memecahkan masalah akses folder publik menggunakan Outlook.
 
**Untuk mengontrol pengguna mana yang bisa mengakses folder publik menggunakan Outlook:**

1.  Gunakan Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true atau $false  
      
    $true: Izinkan pengguna mengakses folder publik di Outlook  
      
    $false: Cegah pengguna mengakses folder publik di Outlook. Ini adalah nilai default.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Catatan** Prosedur ini hanya bisa mengontrol koneksi dengan desktop Outlook untuk Windows klien. Pengguna bisa terus mengakses folder publik menggunakan OWA atau Outlook untuk Mac.
 
Untuk informasi selengkapnya, [lihat Mengumumkan Dukungan untuk Koneksi Terkontrol ke Folder Publik di Outlook](https://aka.ms/controlpf).