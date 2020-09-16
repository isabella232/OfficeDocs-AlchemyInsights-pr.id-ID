---
title: Pemecahan masalah acara dari email
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658737"
---
# <a name="troubleshooting-events-from-email"></a>Pemecahan masalah acara dari email

1. Verifikasi fitur diaktifkan untuk kotak surat: **Get-EventsFromEmailConfiguration-identitas <mailbox> **

2. Lalu lihat ' acara dari email ' log **Export-MailboxDiagnosticLogs <mailbox> -component timeprofile**

3. Dalam log ' acara dari email ', temukan InternetMessageId yang cocok dengan item dalam kotak surat.  

4. Nilai Trustmenentukan Apakah item ditambahkan atau tidak. Acara hanya akan ditambahkan jika TrustScore = "Trusted".

TrustScore ditentukan oleh SPF, DKIM atau properti dMarc, yang berada di header pesan.

Untuk menampilkan properti ini:

**Outlook desktop**

- Membuka item
- Properti file->-header Internet >

atau

**MFCMapi**

- Menavigasi ke item dalam kotak masuk
- Cari PR_TRANSPORT_MESSAGE_HEADERS_W

Properti ini ditentukan dan direkam selama pengangkutan dan perutean. Untuk pemecahan masalah lebih lanjut, Anda mungkin perlu menindaklanjuti dukungan transportasi tentang kegagalan SPF, DKIM, dan. or DMARC.