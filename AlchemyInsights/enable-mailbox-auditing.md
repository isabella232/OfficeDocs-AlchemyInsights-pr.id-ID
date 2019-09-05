---
title: Mengaktifkan audit kotak pesan
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736256"
---
# <a name="enable-mailbox-auditing"></a>Mengaktifkan audit kotak pesan

Untuk mengaktifkan audit kotak surat untuk salah satu pengguna atau seluruh organisasi cmdlet berikut harus dijalankan dari remote Power Shell:
  
 **Pengguna tunggal**
  
Set-kotak surat-identitas "Jane Dow"-AuditEnabled $true
  
 **Organisasi**
  
Get-kotak surat-ResultSize terbatas-filter {RecipientTypeDetails-EQ "UserMailbox"} | Set-kotak surat-AuditEnabled $true
  
[Pelajari lebih lanjut](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

