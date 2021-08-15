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
ms.openlocfilehash: b134c952e3cc5305d8f3e6f44031e7f33d7938b67ff122c46cb74bbd33cbf59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994868"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Mengatur ClientAccessServerEnabled ke True

Jika Tidak dapat membuka pesan email terenkripsi dan sebagai gantinya, lihat lampiran **rpmsg,** lakukan langkah-langkah berikut:

1. Koneksi ke Exchange Online PowerShell.

> [!NOTE]
> Untuk menyambungkan ke Exchange Online PowerShell, Anda harus masuk menggunakan admin global atau Exchange admin.

   a. Buka Windows PowerShell, lalu jalankan perintah berikut:`$UserCredential = Get-Credential`
b. Dalam kotak **dialog Windows PowerShell Permintaan Kredensial,** masukkan akun kerja atau sekolah dan kata sandi, c. Klik **OK**. 

2. Jalankan perintah berikut ini untuk membuat sesi baru:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Jalankan perintah berikut:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Perintah `Get-IRMConfiguration` Jalankan.

4. Periksa pengaturan **ClientAccessServerEnabled.** 

    a. Jika **pengaturan ClientAccessServerEnabled** diatur ke **False,** jalankan cmdlet berikut: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Selalu tutup sesi powershell dengan perintah berikut: `Remove-PSSession $Session`

Untuk informasi selengkapnya, lihat [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

