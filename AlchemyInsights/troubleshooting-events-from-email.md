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
ms.openlocfilehash: b6a8b2a1174f04a1e0ed0fdee9a954bb3bf108038f0804353d84755e490f5f47
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105355"
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