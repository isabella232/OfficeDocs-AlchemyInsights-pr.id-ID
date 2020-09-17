---
title: Perlu menandai domain atau pengirim email yang aman?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803248"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Perlu menandai domain atau pengirim email yang aman?

- Penggunaan **daftar pengirim aman tidak disarankan** karena membuka organisasi Anda ke spam, Phish, dan spoofing.
- Namun, jika ada persyaratan bisnis, **sebaiknya gunakan** **[aturan alur email](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** untuk ini. Panduan kami memastikan autentikasi pengirim (verifikasi pengiriman domain tidak bersifat palsu). **Catatan**: kami tidak menyarankan mengelola false positive dengan menggunakan daftar pengirim aman, karena pengecualian untuk pemfilteran spam bisa membuka organisasi Anda untuk serangan keamanan. Jika pengguna Anda menerima pesan yang salah ditandai sebagai email spam atau junk, silakan **[Laporkan pesan dan file ke Microsoft](https://protection.office.com/reportsubmission)**.
- Pengirim aman di Outlook, daftar pengirim yang diperbolehkan, atau daftar domain yang diperbolehkan dalam kebijakan anti spam **harus dihindari** karena pengirim melewati semua spam, spoof, dan proteksi Phish, serta autentikasi pengirim (SPF, DKIM, dMarc). Metode ini paling baik digunakan untuk uji sementara saja.
