---
title: Pengiriman email yang diblokir oleh SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 7d6ad2667613ae948a4abcefafe8d91cf89d2418
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402262"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Pengiriman email: host klien yang diblokir menggunakan Spamhaus

Alamat IP yang mengirim pesan adalah pada daftar blokir yang dimiliki oleh [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Alasan untuk diblokir oleh Spamhaus menyertakan account dikompromikan, dikompromikan mesin berbagi alamat IP publik, dan kebijakan Internet Service Provider (ISP). Perbaikan yang mungkin adalah:
  
- Diblokir inbound pesan ke Office 365 mana Anda kontrol sumber server email, Anda perlu untuk menentukan penyebab dan menghapus blok dari situs Spamhaus.
    
- Diblokir inbound pesan ke Office 365 mana alamat IP sumber milik orang lain, pemilik alamat kebutuhan untuk menghapus blok dari situs Spamhaus. Jika alamat IP pada kebijakan blok daftar (PBL), pemilik dapat menetapkan alamat IP statis yang berbeda atau menghapus alamat dari PBL.
    
- Untuk pesan keluar diblokir dari domain Office 365, Anda dapat menerima kesalahan ini jika pesan akan diteruskan melalui layanan pihak ke-3. Anda dapat menggunakan alat pencarian WHOIS untuk menemukan pemilik alamat IP yang diblokir.
    

