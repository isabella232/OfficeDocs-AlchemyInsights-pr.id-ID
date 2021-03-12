---
title: Setel ClientAccessServerEnabled ke True
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
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746413"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Setel ClientAccessServerEnabled ke True

Jika Anda tidak bisa membuka pesan email terenkripsi dan sebagai gantinya melihat lampiran **MSG** , lakukan langkah-langkah berikut:

1. Menyambungkan ke Exchange Online PowerShell.

> [!NOTE]
> Untuk menyambungkan ke Exchange Online PowerShell, Anda harus masuk menggunakan akun admin global atau Exchange admin.

   untuk. Buka Windows PowerShell, lalu jalankan perintah berikut: `$UserCredential = Get-Credential`
b. Dalam kotak dialog **permintaan kredensial Windows PowerShell** , masukkan akun kerja atau sekolah dan kata sandi Anda, c. Klik **OK**. 

2. Jalankan perintah berikut ini untuk membuat sesi baru:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    untuk. Jalankan perintah berikut:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Jalankan `Get-IRMConfiguration` perintah.

4. Periksa pengaturan **Clientaccessserverenabled** . 

    untuk. Jika pengaturan **Clientaccessserverenabled** diatur ke **false**, Jalankan cmdlet berikut: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Selalu tutup sesi PowerShell Anda dengan perintah berikut ini: `Remove-PSSession $Session`

Untuk informasi selengkapnya, lihat [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

