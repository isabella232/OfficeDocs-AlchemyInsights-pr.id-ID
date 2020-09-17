---
title: Kesalahan pengiriman email diblokir oleh SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783806"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Kesalahan mengirim email: host klien diblokir menggunakan SpamHaus

Alamat IP yang mengirim pesan ada di daftar blokir yang dimiliki oleh [SpamHaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Alasan diblokir oleh SpamHaus termasuk akun yang dikompromikan, Mesin disusupi berbagi alamat IP publik, dan kebijakan penyedia layanan internet (ISP). Kemungkinan perbaikan adalah:
  
- Untuk pesan masuk yang diblokir tempat Anda mengontrol server email sumber, Anda harus menentukan penyebabnya dan menghapus blok dari situs web SpamHaus.

- Untuk pesan masuk yang diblokir tempat alamat IP sumber milik orang lain, pemilik alamat harus menghapus blok dari situs web SpamHaus. Jika alamat IP berada di daftar blokir kebijakan (PBL), pemilik dapat menetapkan alamat IP statis berbeda atau menghapus alamat dari PBL.

- Untuk pesan keluar yang diblokir dari domain Anda yang tersambung ke Microsoft, Anda bisa menerima kesalahan ini jika pesan dirutekan melalui layanan pihak ketiga. Anda dapat menggunakan alat pencarian WHOIS untuk menemukan pemilik alamat IP yang diblokir.
