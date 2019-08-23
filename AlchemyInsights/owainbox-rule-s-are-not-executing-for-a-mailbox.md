---
title: 1332 OWA - Inbox Bapepam tidak mengeksekusi untuk kotak pesan
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 901237d4dc7b99695097142c61a4bfef7c09750d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36555776"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Aturan kotak masuk tidak bekerja seperti yang diharapkan

Pastikan pengaturan berikut di Outlook di web:

- Pesan dapat diarahkan, diteruskan, atau menjawab secara otomatis berdasarkan aturan kotak masuk hanya satu kali. Aturan pengarah ulang (aturan kotak masuk atau pesan aliran aturan, juga dikenal sebagai aturan transport) dapat menambahkan maksimal sepuluh penerusan penerima pesan. Untuk selengkapnya, lihat [batas aturan jurnal, transportasi, dan kotak masuk](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- Aturan kotak masuk tidak bekerja pada kotak pesan alternatif Journal. Untuk selengkapnya tentang kotak pesan alternatif Journal, lihat [kotak pesan jurnal alternatif](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Untuk mengatasi masalah ini, lihat [KB 2829319](https://support.microsoft.com/kb/2829319).

Jika masalah-masalah sebelumnya tidak berlaku, jalankan laporan diagnostik aturan kotak masuk sebelum Anda meneruskan masalah tersebut ke Microsoft Support:

1. Membuka kotak pesan di Outlook di web, dan klik <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Pengaturan** > **Lihat semua pengaturan Outlook** > **pos** > **aturan**.

2. Di bagian bawah laman, klik **jika aturan tidak bekerja klik di sini untuk menghasilkan laporan diagnostik**.
