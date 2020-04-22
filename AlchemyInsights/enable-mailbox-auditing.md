---
title: Mengaktifkan audit kotak pesan
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: ae11d6be0789a5662d202b85268480a3d42922c4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703574"
---
# <a name="enable-mailbox-auditing"></a>Mengaktifkan audit kotak pesan

Untuk mengaktifkan audit kotak surat untuk salah satu pengguna atau seluruh organisasi cmdlet berikut harus dijalankan dari remote Power Shell:
  
 **Pengguna tunggal**
  
Set-kotak surat-identitas "Jane Dow"-AuditEnabled $true
  
 **Organisasi**
  
Get-kotak surat-ResultSize terbatas-filter {RecipientTypeDetails-EQ "UserMailbox"} | Set-kotak surat-AuditEnabled $true
  
[Pelajari lebih lanjut](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

