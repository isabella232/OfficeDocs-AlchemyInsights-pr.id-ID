---
title: Pesan yang dikirim ke grup Microsoft 365 tidak diterima oleh semua anggota
ms.author: pebaum
author: pebaum
manager: mnirkhe
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 080c060f5675065704c7209bd15e4cbb1236b8db
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 03/05/2021
ms.locfileid: "50480686"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>Pesan yang dikirim ke grup Microsoft 365 tidak diterima oleh semua anggota

Pastikan semua anggota grup telah berlangganan untuk menerima email. Lihat [Mengikuti grup di Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).  

Untuk memeriksa status pesan anggota yang telah berlangganan email grup, jalankan perintah berikut di [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

Gunakan perintah EXO PowerShell berikut untuk mengonfigurasi semua anggota grup untuk menerima email yang dikirimkan ke grup Microsoft 365 di kotak masuk mereka:

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

Misalnya:

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`