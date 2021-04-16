---
title: Perlu menandai domain atau pengirim email dengan aman?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792135"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Perlu menandai domain atau pengirim email dengan aman?

- Penggunaan daftar **pengirim aman tidak direkomendasikan karena** membuka organisasi Anda untuk serangan spam, pengelabuan, dan spoofing.
- Namun, jika ada persyaratan bisnis, kami menyarankan **Agar Anda** menggunakan **[Aturan Aliran Email](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** untuk hal ini. Panduan kami memastikan bahwa autentikasi pengirim (memverifikasi bahwa domain yang dikirim tidak merupakan spoofed). **Catatan**: Kami tidak menyarankan Anda mengelola positif palsu dengan menggunakan daftar pengirim aman, karena pengecualian pemfilteran spam dapat membuka organisasi Anda untuk serangan keamanan. Jika pengguna Anda menerima pesan yang salah ditandai sebagai spam atau email sampah, silakan **[Laporkan pesan dan file ke Microsoft](https://protection.office.com/reportsubmission)**.
- Pengirim Aman di Outlook, Daftar pengirim yang diperbolehkan, atau  daftar domain yang diperbolehkan dalam kebijakan anti spam harus dihindari karena pengirim melewati semua spam, spoof, dan proteksi phish, serta autentikasi pengirim (SPF, DKIM, DMARC). Metode ini paling baik digunakan untuk pengujian sementara saja.
