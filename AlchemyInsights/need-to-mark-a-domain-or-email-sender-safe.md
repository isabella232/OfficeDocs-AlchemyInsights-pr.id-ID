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
ms.openlocfilehash: afc865a7b91036bd2d982e21dce059a87e109e3e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/13/2021
ms.locfileid: "58319951"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Perlu menandai domain atau pengirim email dengan aman?

- Penggunaan daftar **pengirim aman tidak direkomendasikan karena** membuka organisasi Anda untuk serangan spam, pengelabuan, dan spoofing.
- Namun, jika ada persyaratan bisnis, kami menyarankan **agar menggunakan** **[Aturan Flow Email](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** untuk ini. Panduan kami memastikan bahwa autentikasi pengirim (memverifikasi bahwa domain yang dikirim tidak merupakan spoofed). 
    **Catatan**: Kami tidak menyarankan Anda mengelola positif palsu dengan menggunakan daftar pengirim aman, karena pengecualian pemfilteran spam dapat membuka organisasi Anda untuk serangan keamanan. Jika pengguna Anda menerima pesan yang salah ditandai sebagai spam atau email sampah, **[Laporkan pesan dan file ke Microsoft](https://protection.office.com/reportsubmission)**.
- Brankas Daftar pengirim dalam Outlook, Daftar pengirim yang diperbolehkan, atau  daftar domain yang diperbolehkan dalam kebijakan anti spam harus dihindari karena pengirim melewati semua proteksi spam, spoof, dan phish, serta autentikasi pengirim (SPF, DKIM, DMARC). Metode ini paling baik digunakan untuk pengujian sementara saja.
- Validasi bahwa evaluasi Antispam melewati email tertentu bisa dilakukan dengan memeriksa header pesan "X-Forefront-Antispam-Report" (SFV:SFE, SFV:SKA, SFV:SKN), lihat **[Header pesan anti spam.](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)**
- Karena Microsoft ingin menjaga pelanggan kami tetap [aman secara default,](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions)beberapa timpaan penyewa tidak diterapkan untuk malware dan pengelabuan kepercayaan tinggi. Timpaan ini meliputi: o Daftar pengirim yang diperbolehkan atau daftar domain yang diperbolehkan (kebijakan anti spam) Outlook Brankas Pengirim dan Daftar Yang Diizinkan IP (pemfilteran koneksi) 
- Satu-satunya pengesampuan yang memungkinkan pesan pengelabuan (phishing) kepercayaan tinggi untuk melewati pemfilteran adalah Exchange mailflow (juga dikenal sebagai aturan transpor). Untuk menggunakan aturan aliran email untuk melewati pemfilteran, lihat Menggunakan aturan aliran email untuk mengatur tingkat **[kepercayaan spam (SCL) dalam pesan](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)**.