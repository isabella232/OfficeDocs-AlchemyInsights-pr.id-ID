---
title: Memecahkan masalah tips keamanan untuk pemeriksaan deteksi penipuan
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834734"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Memecahkan masalah tips keamanan untuk pemeriksaan deteksi penipuan

Jika Anda mendapatkan tips pengamanan yang mengatakan "Pengirim gagal memeriksa pendeteksian penipuan kami dan mungkin bukan siapa mereka yang ditampilkan", pengirim gagal melewati pemeriksaan autentikasi DKIM atau SPF. Metode terbaik untuk mengatasi masalah ini adalah pengirim dapat mengotorisasi dirinya sendiri. Jika pengirim mengirim atas nama Anda, Anda perlu mengotorisasi mereka dengan menambahkan alamat IP pengirim ke catatan SPF Anda.
  
Lihat [Memecahkan masalah tips keamanan berwarna merah (mencurigakan) untuk pemeriksaan deteksi](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) penipuan untuk informasi selengkapnya.
  
Berikut adalah beberapa tautan lain yang dapat membantu:
  
- [Bagaimana Microsoft menggunakan kerangka kebijakan pengirim (SPF) untuk mencegah spoofing](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Menyiapkan SPF untuk membantu mencegah spoofing](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
