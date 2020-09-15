---
title: Pemecahan masalah Tips keamanan untuk pemeriksaan deteksi penipuan
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: e42b498070bf5d9bfc36110667da8cc0fd431524
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658413"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Pemecahan masalah Tips keamanan untuk pemeriksaan deteksi penipuan

Jika Anda mendapatkan tips keselamatan yang mengatakan "pengirim gagal memeriksa deteksi penipuan kami dan mungkin bukan sebagai siapa mereka terlihat", maka pengirim gagal melewati pemeriksaan autentikasi DKIM atau SPF. Metode terbaik untuk mengatasi masalah ini adalah agar pengirim mengotorisasi dirinya. Jika pengirim mengirim atas nama Anda, Anda perlu mengotorisasi mereka dengan menambahkan alamat IP pengirim ke catatan SPF Anda.
  
Lihat [pemecahan masalah Tips keamanan berwarna merah (mencurigakan) untuk pemeriksaan deteksi penipuan](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) untuk informasi selengkapnya.
  
Berikut adalah beberapa tautan lain yang dapat membantu:
  
- [Cara Microsoft menggunakan Sender Policy Framework (SPF) untuk mencegah spoofing](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Menyiapkan SPF untuk membantu mencegah spoofing](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
