---
title: Tidak dapat mengakses folder publik
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
- "3500007"
- "3462"
ms.openlocfilehash: 272918b38f6019cb2bdcaa4013baebaa5f04fe85
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812550"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook tidak dapat tersambung ke folder publik

Jika akses folder publik tidak berfungsi untuk beberapa pengguna, cobalah hal berikut:

Sambungkan ke EXO PowerShell dan konfigurasikan parameter DefaultPublicFolderMailbox pada akun pengguna bermasalah untuk mencocokkan parameter pada akun pengguna yang bekerja.

Misalnya

Dapatkan-kotak surat pengguna | Kotak surat ft Defaultpublicfolder, EffectivePublicFolderMailbox

Set-kotak surat ProblemUser-DefaultPublicFolderMailbox \<value from previous command>

Tunggu setidaknya satu jam agar perubahan diterapkan.

Jika masalah tetap terjadi, ikuti [prosedur ini](https://aka.ms/pfcte) untuk memecahkan masalah akses folder publik menggunakan Outlook.
 
**Untuk mengontrol pengguna mana yang bisa mengakses folder publik menggunakan Outlook**:

1.  Menggunakan Set-CASMailbox <mailboxname> -publicfolderclientaccess $True atau $false  
      
    $true: Izinkan pengguna mengakses folder publik di Outlook  
      
    $false: mencegah akses pengguna ke folder publik di Outlook. Ini adalah nilai default.  
        
2.  Set-OrganizationConfig-PublicFolderShowClientControl $true   
      
**Catatan** Prosedur ini hanya dapat mengontrol koneksi dengan klien Outlook desktop untuk Windows. Pengguna bisa terus mengakses folder publik menggunakan OWA atau Outlook untuk Mac.
 
Untuk informasi selengkapnya, lihat [mengumumkan dukungan untuk koneksi terkendali ke folder publik di Outlook](https://aka.ms/controlpf).