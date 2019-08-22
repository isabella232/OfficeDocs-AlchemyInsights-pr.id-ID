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
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 7ce8bcc7caefebf51fc8d9622367fd16405deef1
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36533186"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Pemecahan masalah tip keselamatan untuk deteksi penipuan cek

Jika Anda mendapatkan tip keselamatan yang mengatakan "pengirim gagal pemeriksaan deteksi penipuan kami dan tidak mungkin yang mereka tampak", kemudian pengirim gagal dalam mewariskan DKIM atau SPF otentikasi cek. Metode terbaik untuk memecahkan masalah ini adalah untuk pengirim untuk mengotorisasi sendiri. Jika pengirim mengirim atas nama Anda, Anda perlu wewenang mereka dengan menambahkan alamat IP pengirim ke record SPF Anda.
  
Lihat [pemecahan masalah merah (mencurigakan) safety Tips untuk deteksi penipuan cek](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) untuk info lebih lanjut.
  
Berikut adalah beberapa link yang dapat membantu:
  
- [Bagaimana Office 365 menggunakan kerangka kebijakan pengirim (SPF) untuk mencegah spoofing](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [Mengatur SPF di Office 365 untuk membantu mencegah spoofing](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
