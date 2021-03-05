---
title: Mengaktifkan pengauditan kotak surat
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: aa0ff925ae891d28e31394ec66eb17c2d9710008
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482470"
---
# <a name="turn-on-mailbox-auditing"></a>Mengaktifkan pengauditan kotak surat

Untuk mengaktifkan pengauditan kotak surat untuk pengguna tunggal atau seluruh organisasi, Jalankan cmdlet berikut dari remote PowerShell:

- **Pengguna tunggal**: Set-Mailbox-identitas "Jane Dow"-auditenabled $True
- **Organisasi**: Get-Mailbox-ResultSize Unlimited-filter {RecipientTypeDetails-EQ "UserMailbox"} | Set-Mailbox-AuditEnabled $true

Untuk mempelajari selengkapnya, lihat [mengelola audit kotak surat](https://go.microsoft.com/fwlink/?linkid=2103668).