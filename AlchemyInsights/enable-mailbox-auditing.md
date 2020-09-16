---
title: Mengaktifkan pengauditan kotak surat
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 404ef9ecd824541f98471bb8797f5f6e025012b7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806294"
---
# <a name="enable-mailbox-auditing"></a>Mengaktifkan pengauditan kotak surat

Untuk mengaktifkan pengauditan kotak surat baik untuk satu pengguna atau seluruh organisasi, cmdlet berikut harus dijalankan dari remote Power Shell:
  
 **Pengguna tunggal**
  
Set-kotak surat-identitas "Jane Dow"-AuditEnabled $true
  
 **Ulang**
  
Get-kotak surat-ResultSize Unlimited-filter {RecipientTypeDetails-EQ "UserMailbox"} | Set-kotak surat-AuditEnabled $true
  
[Pelajari lebih lanjut](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

