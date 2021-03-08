---
title: Menggunakan Exchange Online PowerShell untuk mengaktifkan DKIM untuk domain tertentu
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
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524177"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Menggunakan Exchange Online PowerShell untuk mengaktifkan DKIM untuk domain tertentu

Jika Anda tidak dapat membuat catatan DNS DKIM di pusat admin, coba gunakan Exchange Online PowerShell. 

Untuk membuat catatan DNS DKIM menggunakan Exchange Online PowerShell, lakukan langkah-langkah berikut:

1. Buka Windows PowerShell sebagai administrator dan jalankan perintah berikut dalam urutan yang dijelaskan:

    untuk. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    's. `Import-PSSession $Session -DisableNameChecking`
    
Jika Anda mengalami masalah saat menyambungkan ke Exchange Online PowerShell, lihat [menyambungkan ke Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

2. Setelah Anda tersambung ke Exchange Online PowerShell, jalankan perintah berikut:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Setelah perintah di atas berhasil dieksekusi, jalankan perintah berikut ini untuk mengakhiri sesi PowerShell Exchange Online:

    `Remove-PSSession $Session` 



