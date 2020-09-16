---
title: Masalah aktivasi-kami tidak dapat menyambungkan sekarang
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725986"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Memperbaiki aplikasi Microsoft 365 "kami tidak dapat menyambungkan sekarang" pesan

Jika Anda menerima pesan ini, cobalah hal berikut:

1. Periksa firewall, perangkat lunak antivirus, dan pengaturan proksi Anda untuk mengonfirmasi bahwa mereka tidak memblokir akses internet ke aplikasi Microsoft 365. Lihat [Microsoft URL dan rentang alamat IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Masuk ke **mulai**  >  **Jalankan**, lalu ketikkan **Services. MSC**. Pastikan bahwa layanan berikut ini berjalan:
    - Penyetelan otomatis perangkat yang tersambung ke jaringan
    - Layanan daftar jaringan
    - Kesadaran lokasi jaringan
    - Log kejadian Windows

Jika salah satu layanan ini tidak berjalan, cobalah untuk memulainya. Jika Anda mengalami masalah memulai layanan, jalankan perintah berikut ini dengan membuka perintah dengan izin yang ditinggikan:

**SFC/SCANNOW**

Setelah perintah ini selesai, mulai ulang komputer.

Untuk informasi mendetail, lihat ["Maaf, kami tidak dapat tersambung ke akun Anda. Kesalahan coba lagi nanti "saat Anda mengaktifkan Office dari Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).