---
title: Mengatur ClientAccessServerEnabled ke True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: fc953813a94c9ed3226f81f776d6085e12a6cafc
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320359"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Mengatur ClientAccessServerEnabled ke True

Jika Tidak dapat membuka pesan email terenkripsi dan sebagai gantinya, lihat lampiran **rpmsg,** lakukan langkah-langkah berikut:

1. Koneksi ke Exchange Online PowerShell.

    **Catatan**: Untuk tersambung Exchange Online PowerShell, Anda harus masuk menggunakan admin global atau Exchange admin global.

   a. Buka Windows PowerShell, lalu jalankan perintah berikut:`$UserCredential = Get-Credential`
   b. Dalam kotak **dialog Windows PowerShell Permintaan Kredensial,** masukkan akun kerja atau sekolah dan kata sandi Anda, c. Klik **OK**. 

2. Jalankan perintah berikut ini untuk membuat sesi baru:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Jalankan perintah berikut:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Perintah `Get-IRMConfiguration` Jalankan.

4. Periksa pengaturan **ClientAccessServerEnabled.** 

    a. Jika **pengaturan ClientAccessServerEnabled** diatur ke **False,** jalankan cmdlet berikut: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

**Tips**: Selalu tutup sesi powershell dengan perintah berikut: `Remove-PSSession $Session`

Untuk informasi selengkapnya, [lihat Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

