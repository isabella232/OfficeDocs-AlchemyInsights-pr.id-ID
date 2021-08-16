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
ms.openlocfilehash: 797dd57aaa43e879c015a36c79c8c9fb13e04ae894b33b0f7c6d9694d1ae1960
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058041"
---
# <a name="turn-on-mailbox-auditing"></a>Mengaktifkan pengauditan kotak surat

Untuk mengaktifkan pengauditan kotak surat untuk satu pengguna atau seluruh organisasi, jalankan cmdlet berikut dari PowerShell Jarak Jauh:

- **Pengguna tunggal**: Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true
- **Organisasi**: Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true

Untuk mempelajari selengkapnya, lihat [Mengelola pengauditan kotak surat](https://go.microsoft.com/fwlink/?linkid=2103668).