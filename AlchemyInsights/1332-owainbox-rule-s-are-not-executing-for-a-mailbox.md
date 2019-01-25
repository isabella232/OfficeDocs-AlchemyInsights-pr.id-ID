---
title: 1332 OWA - Inbox Bapepam tidak mengeksekusi untuk kotak pesan
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: f090d0a9d84bc6a4d1a1f4c0af55102d4b0ddfbe
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/24/2019
ms.locfileid: "29475125"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Aturan kotak masuk tidak bekerja seperti yang diharapkan

Pastikan pengaturan berikut:
  
- Pesan dapat diarahkan, diteruskan, atau menjawab secara otomatis berdasarkan aturan kotak masuk hanya satu kali. Aturan pengarah ulang (aturan kotak masuk atau pesan aliran aturan, juga dikenal sebagai aturan transport) dapat menambahkan maksimal sepuluh penerusan penerima pesan. Untuk selengkapnya, lihat [batas aturan jurnal, transportasi, dan kotak masuk](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).
    
- Aturan kotak masuk tidak bekerja pada kotak pesan alternatif Journal. Untuk selengkapnya tentang kotak pesan alternatif Journal, lihat [kotak pesan jurnal alternatif](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).
    
Untuk mengatasi masalah ini, lihat [KB 2829319](https://support.microsoft.com/kb/2829319).
  
Jika masalah-masalah sebelumnya tidak berlaku, jalankan laporan diagnostik aturan kotak masuk sebelum Anda meneruskan masalah tersebut ke Microsoft Support:
  
1. Membuka kotak pesan di Outlook di web, lalu klik **pengaturan** \> **pilihan** \> **mengatur email** \> **aturan kotak masuk**.
    
2. Di bagian bawah laman, klik **jika aturan tidak bekerja klik di sini untuk menghasilkan laporan diagnostik**.
    

