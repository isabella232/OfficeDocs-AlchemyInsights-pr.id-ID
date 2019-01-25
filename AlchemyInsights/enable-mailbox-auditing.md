---
title: Mengaktifkan kotak pesan audit
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: bd94ec10f9df2e72ec6e3d8552d2eb80212a9d78
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/24/2019
ms.locfileid: "29500285"
---
# <a name="enable-mailbox-auditing"></a>Mengaktifkan kotak pesan audit

Aktifkan kotak pesan audit untuk pengguna tunggal atau seluruh organisasi cmdlet berikut harus dijalankan dari Remote Power Shell:
  
 **Satu pengguna**
  
Set-kotak surat - identitas "Jane Dow" - AuditEnabled $true
  
 Organization
  
Get-kotak surat - ResultSize Unlimited - Filter {RecipientTypeDetails - persamaan "UserMailbox"} | Set-kotak surat - AuditEnabled $true
  
[Pelajari lebih lanjut](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  

