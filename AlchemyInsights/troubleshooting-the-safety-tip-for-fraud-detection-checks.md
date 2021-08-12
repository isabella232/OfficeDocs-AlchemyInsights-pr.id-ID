---
title: Memecahkan masalah kiat keamanan untuk pemeriksaan deteksi penipuan
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
ms.openlocfilehash: c7ee1fcc887a3221b5f2acda1aa6ae6beb03cb96686d4ecb7828a02f8ff48302
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955969"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Memecahkan masalah kiat keamanan untuk pemeriksaan deteksi penipuan

Jika Anda mendapatkan pesan kiat keamanan yang mengatakan "Pengirim gagal memeriksa pendeteksian penipuan kami dan mungkin bukan siapa mereka yang ditampilkan", pengirim gagal melewati pemeriksaan autentikasi DKIM atau SPF. Metode terbaik untuk mengatasi masalah ini adalah pengirim dapat mengotorisasi dirinya sendiri. Jika pengirim mengirim atas nama Anda, Anda perlu mengotorisasi mereka dengan menambahkan alamat IP pengirim ke catatan SPF Anda.
  
Lihat [Memecahkan masalah warna merah (mencurigakan) kiat keamanan untuk pendeteksian penipuan memeriksa](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) informasi selengkapnya.
  
Berikut adalah beberapa tautan lain yang dapat membantu:
  
- [Bagaimana Microsoft menggunakan kerangka kebijakan pengirim (SPF) untuk mencegah spoofing](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Menyiapkan SPF untuk membantu mencegah spoofing](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
