---
title: Mengatasi masalah tip keselamatan untuk pemeriksaan pendeteksian penipuan
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 74913492a086de688067d588e95dd87e6946743b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/02/2020
ms.locfileid: "44504986"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Mengatasi masalah tip keselamatan untuk pemeriksaan pendeteksian penipuan

Jika Anda mendapatkan tip keselamatan yang berbunyi "pengirim gagal memeriksa deteksi penipuan kami dan mungkin tidak menjadi siapa mereka tampaknya", maka pengirim gagal untuk lulus baik DKIM atau SPF otentikasi cek. Metode terbaik untuk menyelesaikan ini adalah untuk pengirim untuk mengotorisasi diri mereka sendiri. Jika pengirim mengirimkan atas nama Anda, Anda perlu mengotorisasi mereka dengan menambahkan alamat IP pengirim ke data SPF.
  
Lihat [mengatasi masalah Tips keamanan merah (mencurigakan) untuk pemeriksaan deteksi penipuan](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) untuk info lebih lanjut.
  
Berikut adalah beberapa link lain yang dapat membantu:
  
- [Bagaimana Microsoft menggunakan kerangka kebijakan pengirim (SPF) untuk mencegah spoofing](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Menyiapkan SPF untuk membantu mencegah spoofing](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
