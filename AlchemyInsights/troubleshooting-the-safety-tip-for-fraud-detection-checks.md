---
title: Pemecahan masalah tip keselamatan untuk deteksi penipuan cek
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.openlocfilehash: 24842e8cc5c6e47fb0eb637e6a3211637ede1ed8
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/15/2019
ms.locfileid: "28295357"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Pemecahan masalah tip keselamatan untuk deteksi penipuan cek

Jika Anda mendapatkan tip keselamatan yang mengatakan "pengirim gagal pemeriksaan deteksi penipuan kami dan tidak mungkin yang mereka tampak", kemudian pengirim gagal dalam mewariskan DKIM atau SPF otentikasi cek. Metode terbaik untuk memecahkan masalah ini adalah untuk pengirim untuk mengotorisasi sendiri. Jika pengirim mengirim atas nama Anda, Anda perlu wewenang mereka dengan menambahkan alamat IP pengirim ke record SPF Anda.
  
Lihat [pemecahan masalah merah (mencurigakan) safety Tips untuk deteksi penipuan cek](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) untuk info lebih lanjut. 
  
Berikut adalah beberapa link yang dapat membantu:
  
- [Bagaimana Office 365 menggunakan kerangka kebijakan pengirim (SPF) untuk mencegah spoofing](https://docs.microsoft.com/en-us/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)
    
- [Mengatur SPF di Office 365 untuk membantu mencegah spoofing](https://docs.microsoft.com/en-us/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
    

