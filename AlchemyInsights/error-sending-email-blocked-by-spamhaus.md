---
title: Error saat mengirim email yang diblokir oleh SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714261"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Kesalahan pengiriman email: host klien diblokir menggunakan SpamHaus

Alamat IP yang mengirim pesan adalah pada daftar blokir milik [SpamHaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Alasan diblokir oleh SpamHaus termasuk akun yang dikompromikan, dikompromikan mesin berbagi alamat IP publik, dan Internet Service Provider (ISP) kebijakan. Kemungkinan perbaikan adalah:
  
- Untuk pesan masuk diblokir di mana Anda mengontrol server email sumber, Anda perlu menentukan penyebabnya dan menghapus blok dari situs web SpamHaus.

- Untuk pesan masuk diblokir di mana alamat IP sumber milik orang lain, pemilik alamat harus menghapus blok dari situs web SpamHaus. Jika alamat IP di kebijakan blok daftar (PBL), pemilik dapat menetapkan alamat IP statis yang berbeda atau menghapus alamat dari PBL.

- Untuk diblokir pesan keluar dari domain Anda terhubung ke Microsoft, Anda dapat menerima galat ini jika pesan diarahkan melalui layanan pihak ke-3. Anda dapat menggunakan alat pencarian WHOIS untuk menemukan pemilik alamat IP yang diblokir.
