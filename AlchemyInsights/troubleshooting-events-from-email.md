---
title: Pemecahan masalah acara dari email
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569139"
---
# <a name="troubleshooting-events-from-email"></a>Pemecahan masalah acara dari email

1. Verifikasi fitur diaktifkan untuk kotak surat: **Get-EventsFromEmailConfiguration-identitas <mailbox> **

2. Kemudian lihat di ' Events dari email ' log **ekspor-MailboxDiagnosticLogs <mailbox> -komponen timeprofile**

3. Di log "peristiwa dari email", Cari InternetMessageId yang cocok dengan item di kotak pesan.  

4. Yang TrustScore menentukan apakah item yang ditambahkan atau tidak. Acara hanya akan ditambahkan jika TrustScore = "Trusted".

TrustScore ditentukan oleh properti SPF, DKIM atau dMarc, yang berada di header pesan.

Untuk melihat properti ini:

**Desktop Outlook**

- Membuka item
- Properti > file-header Internet >

Atau

**MFCMapi**

- Menavigasi ke item di kotak masuk
- Cari PR_TRANSPORT_MESSAGE_HEADERS_W

Properti ini ditentukan dan direkam selama transportasi dan perutean. Untuk pemecahan masalah lebih lanjut, Anda mungkin perlu menindaklanjuti dengan dukungan transportasi tentang kegagalan dalam SPF, DKIM dan. atau DMARC.