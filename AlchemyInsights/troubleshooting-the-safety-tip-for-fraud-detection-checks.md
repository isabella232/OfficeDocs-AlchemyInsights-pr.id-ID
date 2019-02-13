---
title: Pemecahan masalah tip keselamatan untuk deteksi penipuan cek
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.openlocfilehash: 98627edcd2b685673dda8a8a18821eddf9b64bc1
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/12/2019
ms.locfileid: "29936363"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Pemecahan masalah tip keselamatan untuk deteksi penipuan cek



Jika Anda mendapatkan tip keselamatan yang mengatakan "pengirim gagal pemeriksaan deteksi penipuan kami dan tidak mungkin yang mereka tampak", kemudian pengirim gagal dalam mewariskan DKIM atau SPF otentikasi cek. Metode terbaik untuk memecahkan masalah ini adalah untuk pengirim untuk mengotorisasi sendiri. Jika pengirim mengirim atas nama Anda, Anda perlu wewenang mereka dengan menambahkan alamat IP pengirim ke record SPF Anda.
  
Lihat [pemecahan masalah merah (mencurigakan) safety Tips untuk deteksi penipuan cek](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) untuk info lebih lanjut. 
  
Berikut adalah beberapa link yang dapat membantu:
  
- [Bagaimana Office 365 menggunakan kerangka kebijakan pengirim (SPF) untuk mencegah spoofing](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)
    
- [Mengatur SPF di Office 365 untuk membantu mencegah spoofing](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
    

