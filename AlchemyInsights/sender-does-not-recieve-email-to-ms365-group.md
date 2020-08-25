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
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>Pengirim tidak menerima email yang dikirim ke grup Microsoft 365

Secara default, pengirim pesan email ke grup Microsoft 365 tidak menerima salinan pesan di kotak masuk mereka, meskipun pengirim adalah anggota grup.

Gunakan perintah EXO PowerShell ini untuk memperbolehkan pengirim menerima salinan setiap email yang mereka kirim ke grup Microsoft 365:  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

Untuk mengaktifkan pengaturan untuk semua kotak surat sekaligus:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**Catatan** Perubahan pada pengaturan ini memakan waktu hingga satu jam agar diterapkan.