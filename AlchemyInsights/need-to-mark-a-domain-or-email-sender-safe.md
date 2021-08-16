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
ms.openlocfilehash: 7058b6419e52fce94f3359d0bd8e1d67c5aa5ef6743abf4ed39f45bad49e1d07
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54025613"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Perlu menandai domain atau pengirim email dengan aman?

- Penggunaan daftar **pengirim aman tidak direkomendasikan karena** membuka organisasi Anda untuk serangan spam, pengelabuan, dan spoofing.
- Namun, jika ada persyaratan bisnis, kami menyarankan **agar menggunakan** **[Aturan Flow Email untuk](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** ini. Panduan kami memastikan bahwa autentikasi pengirim (memverifikasi bahwa domain yang dikirim tidak merupakan spoofed). **Catatan**: Kami tidak menyarankan Anda mengelola positif palsu dengan menggunakan daftar pengirim aman, karena pengecualian pemfilteran spam dapat membuka organisasi Anda untuk serangan keamanan. Jika pengguna Anda menerima pesan yang salah ditandai sebagai spam atau email sampah, silakan **[Laporkan pesan dan file ke Microsoft](https://protection.office.com/reportsubmission)**.
- Brankas Pengirim dalam Outlook, Daftar pengirim yang diperbolehkan, atau daftar  domain yang diperbolehkan dalam kebijakan anti spam harus dihindari karena pengirim melewati semua proteksi spam, spoof, dan phish, serta autentikasi pengirim (SPF, DKIM, DMARC). Metode ini paling baik digunakan untuk pengujian sementara saja.
- Validasi bahwa email tertentu yang melewati evaluasi Antispam bisa dilakukan dengan mencentang header pesan "X-Forefront-Antispam-Report" (SFV:SFE, SFV:SKA, SFV:SKN), lihat **[Header pesan anti spam.](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)**
- Karena Microsoft ingin menjaga pelanggan kami tetap [aman secara default,](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions)beberapa timpaan penyewa tidak diterapkan untuk malware dan pengelabuan kepercayaan tinggi. Timpaan ini meliputi: o Daftar pengirim yang diperbolehkan atau daftar domain yang diperbolehkan (kebijakan anti spam) Outlook Brankas Pengirim o Daftar Yang Diizinkan IP (pemfilteran koneksi) 
- Satu-satunya pengesampuan yang memungkinkan pesan pengelabuan (phishing) kepercayaan tinggi untuk melewati pemfilteran adalah Exchange mailflow (juga dikenal sebagai aturan transpor). Untuk menggunakan aturan aliran email untuk melewati pemfilteran, lihat Menggunakan aturan aliran email untuk mengatur tingkat **[kepercayaan spam (SCL) dalam pesan](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)**.