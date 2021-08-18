---
title: AggregateGroupMailbox NDR penuh diterima untuk email yang dikirim Microsoft 365 grup
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004286"
- "7656"
ms.openlocfilehash: ace8e256e3771f82512abcb9e20b832381eedf80
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315913"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>AggregateGroupMailbox NDR penuh diterima untuk email yang dikirim Microsoft 365 grup

Gunakan perintah EXO Shell berikut ini untuk membuat aturan Exchange guna memindahkan email yang dikirim ke kotak surat grup agregat secara diam-diam:

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

**Catatan**: Ganti alamat SMTP di **-SentTo dengan** alamat SMTP dari kotak surat grup agregat dalam penyewa Anda. Anda bisa mendapatkan alamat SMTP kotak surat grup agregat dari NDR yang diterima.



