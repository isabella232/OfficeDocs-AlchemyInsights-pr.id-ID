---
title: 1332 OWA - Aturan kotak masuk tidak menjalankan kotak surat
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
ms.openlocfilehash: b05ed9f0ee8c18b49b5338c53e67a79f1bf65464385dfa0ebd0639172a1b18f2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040905"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Aturan Kotak Masuk tidak berfungsi seperti yang diharapkan

Verifikasi pengaturan berikut ini di Outlook di web:

- Pesan bisa dialihkan, diteruskan, atau dibalas agar secara otomatis berdasarkan aturan Kotak Masuk hanya satu kali. Aturan pengalihan (aturan Kotak Masuk atau aturan aliran email, juga dikenal sebagai aturan transpor) dapat menambahkan maksimal sepuluh penerima penerusan ke sebuah pesan. Untuk informasi selengkapnya, lihat [Batasan aturan Jurnal, Transportasi, dan Kotak Masuk.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)

- Aturan kotak masuk tidak berfungsi di kotak surat jurnal alternatif. Untuk informasi selengkapnya tentang kotak surat jurnal alternatif, lihat [Kotak surat jurnal alternatif](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Untuk memperbaiki masalah ini, lihat [KB 2829319](https://support.microsoft.com/kb/2829319).

Jika masalah sebelumnya tidak berlaku, jalankan laporan diagnostik aturan Kotak Masuk sebelum meningkatkan masalah ke Dukungan Microsoft:

1. Buka kotak surat dalam Outlook di web, dan klik <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Pengaturan**  >  **Menampilkan semua Outlook Pengaturan**  >  **Email**  >  **Aturan**.

2. Di bagian bawah halaman, klik **Jika aturan Anda tidak berfungsi, klik di sini untuk menghasilkan laporan diagnostik.**
