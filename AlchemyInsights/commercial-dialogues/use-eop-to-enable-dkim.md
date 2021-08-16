---
title: Menggunakan Exchange Online PowerShell untuk mengaktifkan DKIM bagi domain tertentu
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: ba627c6da96624914b858aa09d6eff9de709134c2c986fe363845c5ab2b66434
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070306"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Menggunakan Exchange Online PowerShell untuk mengaktifkan DKIM bagi domain tertentu

Jika tidak dapat membuat catatan DNS DKIM di pusat admin, coba gunakan PowerShell Exchange Online. 

Untuk membuat catatan DNS DKIM menggunakan PowerShell Exchange Online, lakukan langkah-langkah berikut ini:

1. Buka Windows PowerShell sebagai administrator dan jalankan perintah berikut dalam urutan yang diuraikan:

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Jika anda mengalami masalah saat menyambungkan ke Exchange Online PowerShell, [lihat Koneksi ke Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

2. Setelah tersambung ke PowerShell Exchange Online, jalankan perintah berikut:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Setelah perintah di atas berhasil dijalankan, jalankan perintah berikut untuk mengakhiri Exchange Online PowerShell:

    `Remove-PSSession $Session` 



