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
ms.openlocfilehash: d222eb92d806bad52264139a8ddba72f323b3783
ms.sourcegitcommit: 10cfd9d552b0d8a096bcef34e82c04a4c166a13a
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 03/05/2021
ms.locfileid: "50479456"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a><span data-ttu-id="2d579-102">Pesan yang dikirim ke grup Microsoft 365 tidak diterima oleh semua anggota</span><span class="sxs-lookup"><span data-stu-id="2d579-102">Messages sent to a Microsoft 365 group are not received by all members</span></span>

<span data-ttu-id="2d579-103">Pastikan bahwa semua anggota grup telah berlangganan untuk menerima email.</span><span class="sxs-lookup"><span data-stu-id="2d579-103">Make sure that all group members have subscribed to receive the emails.</span></span> <span data-ttu-id="2d579-104">Lihat [Mengikuti grup di Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span><span class="sxs-lookup"><span data-stu-id="2d579-104">See [Follow a group in Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span></span>  

<span data-ttu-id="2d579-105">Untuk memeriksa status pesan anggota yang telah berlangganan email grup, jalankan perintah berikut di [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):</span><span class="sxs-lookup"><span data-stu-id="2d579-105">To check the message status of members who have subscribed to group emails, run the following command on [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):</span></span>

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

<span data-ttu-id="2d579-106">Gunakan perintah EXO PowerShell berikut untuk mengonfigurasi semua anggota grup untuk menerima email yang dikirimkan ke grup Microsoft 365 di kotak masuk mereka:</span><span class="sxs-lookup"><span data-stu-id="2d579-106">Use the following EXO PowerShell command to configure all group members to receive emails sent to Microsoft 365 group in their inbox:</span></span>

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

<span data-ttu-id="2d579-107">Misalnya:</span><span class="sxs-lookup"><span data-stu-id="2d579-107">For example:</span></span>

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`