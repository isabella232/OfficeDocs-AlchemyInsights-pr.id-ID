---
title: Pemecahan Masalah Acara dari Email
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834842"
---
# <a name="troubleshooting-events-from-email"></a>Pemecahan Masalah Acara dari Email

1. Memverifikasi bahwa fitur ini diaktifkan untuk kotak surat: **Get-EventsFromEmailConfiguration -Identity <mailbox>**

2. Lalu lihat log 'Acara dari Email' **Ekspor-Kotak SuratDiagnosticLogs <mailbox> -Component TimeProfile**

3. Dalam log 'Acara dari Email', temukan InternetMessageId yang cocok dengan item dalam kotak surat.  

4. TrustScore menentukan apakah item ditambahkan atau tidak. Acara hanya akan ditambahkan jika TrustScore = "Trusted".

TrustScore ditentukan oleh properti SPF, Dkim atau Dmarc, yang ada di Header Pesan.

Untuk menampilkan properti ini:

**Desktop Outlook**

- Membuka item
- File -> Properti -> Header Internet

atau

**MFCMapi**

- Menavigasi ke item dalam kotak masuk
- Cari PR_TRANSPORT_MESSAGE_HEADERS_W

Properti ini ditentukan dan direkam selama transportasi dan perutean. Untuk pemecahan masalah lebih lanjut, Anda mungkin perlu menindaklanjuti Dukungan Transportasi tentang kegagalan di SPF, DKIM, dan.atau DMARC.