---
title: Pengirim tidak menerima email yang dikirim ke grup Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b3b438e17c35f18289d3e9c3ca89d16a6f2a065f
ms.sourcegitcommit: dcca0df53f9194f406cf3a5f6b046cb33a0a5b03
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/21/2020
ms.locfileid: "46871908"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a><span data-ttu-id="89fb1-102">Pengirim tidak menerima email yang dikirim ke grup Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="89fb1-102">Sender does not receive email sent to Microsoft 365 group</span></span>

<span data-ttu-id="89fb1-103">Secara default, pengirim pesan email ke grup Microsoft 365 tidak menerima salinan pesan di kotak masuk mereka, meskipun pengirim adalah anggota grup.</span><span class="sxs-lookup"><span data-stu-id="89fb1-103">By default, the sender of an email message to a Microsoft 365 group doesn't receive a copy of the message in their Inbox, even if the sender is a member of the group.</span></span>

<span data-ttu-id="89fb1-104">Gunakan perintah EXO PowerShell ini untuk memperbolehkan pengirim menerima salinan setiap email yang mereka kirim ke grup Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="89fb1-104">Use this EXO PowerShell command to allow the sender to receive a copy of each email they send to the Microsoft 365 group:</span></span>  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

<span data-ttu-id="89fb1-105">Untuk mengaktifkan pengaturan untuk semua kotak surat sekaligus:</span><span class="sxs-lookup"><span data-stu-id="89fb1-105">To enable the setting for all mailboxes at once:</span></span>

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

<span data-ttu-id="89fb1-106">**Catatan** Perubahan pada pengaturan ini memakan waktu hingga satu jam agar diterapkan.</span><span class="sxs-lookup"><span data-stu-id="89fb1-106">**Note** Changes to this setting take up to an hour to take effect.</span></span>