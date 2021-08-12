---
title: Kesalahan saat mengirim email yang diblokir oleh SpamHaus
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8372032e19bd2ebaf3ba8cc8e87f19ef3e2edf1e607b1739a919f6dcc443cd97
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946746"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Terjadi kesalahan saat mengirimkan email: Host klien diblokir menggunakan Spamhaus

Alamat IP yang mengirimkan pesan tersebut berada dalam daftar blokir milik [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Alasan pemblokiran yang dilakukan oleh Spamhaus meliputi akun dibobol, komputer yang menggunakan alamat IP publik yang sama dibobol, dan kebijakan Penyedia Layanan Internet (ISP). Perbaikan yang dapat dilakukan adalah:
  
- Untuk pesan masuk yang diblokir tempat Anda mengontrol server email sumber, Anda harus menentukan penyebabnya dan menghapus blokir dari situs web Spamhaus.

- Untuk pesan masuk yang diblokir yang alamat IP sumbernya merupakan milik orang lain, pemilik alamat harus menghapus blokir dari situs web Spamhaus. Jika alamat IP berada dalam Daftar Blokir Kebijakan (PBL), pemilik dapat menetapkan alamat IP statis lain atau menghapus alamat dari PBL.

- Untuk pesan keluar yang diblokir dari domain Anda yang tersambung ke Microsoft, Anda dapat menerima kesalahan ini jika pesan dirutekan melalui layanan pihak ke-3. Anda dapat menggunakan alat pencarian WHOIS untuk menemukan pemilik alamat IP yang diblokir.
