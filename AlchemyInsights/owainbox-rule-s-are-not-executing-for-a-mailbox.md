---
title: 1332 OWA-aturan kotak masuk tidak mengeksekusi untuk kotak surat
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: f4d8db9c590abc490f193ef54a8a1dc5afba82b9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47721594"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Aturan kotak masuk tidak berfungsi seperti yang diharapkan

Verifikasi pengaturan berikut ini di Outlook di web:

- Pesan dapat dialihkan, diteruskan, atau dijawab secara otomatis berdasarkan aturan kotak masuk hanya satu kali. Aturan pengalihan ulang (aturan kotak masuk atau aturan alur email, yang juga dikenal sebagai aturan transpor) bisa menambahkan maksimal 10 Penerima penerusan ke sebuah pesan. Untuk informasi selengkapnya, lihat [batas aturan jurnal, transportasi, dan kotak masuk](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- Aturan kotak masuk tidak berfungsi pada kotak surat penjurnalan alternatif. Untuk informasi selengkapnya tentang kotak surat penjurnalan alternatif, lihat [kotak surat penjurnalan alternatif](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Untuk memperbaiki masalah ini, lihat [KB 2829319](https://support.microsoft.com/kb/2829319).

Jika masalah sebelumnya tidak diterapkan, jalankan laporan diagnostik aturan kotak masuk sebelum Anda meningkatkan masalah ke dukungan Microsoft:

1. Buka kotak surat di Outlook di web, dan klik <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Pengaturan**  >  **Tampilkan semua pengaturan Outlook**  >  **Email**  >  **Aturan**.

2. Di bagian bawah halaman, klik **jika aturan Anda tidak berfungsi klik di sini untuk membuat laporan diagnostik**.
