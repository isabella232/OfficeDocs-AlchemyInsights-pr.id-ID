---
title: Masalah Aktivasi - Kami tidak dapat menyambungkan sekarang
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 5dad4b43efac2468b57351a4d6c96379ed505071ca144ec0aa518e975633bb18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998157"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Memperbaiki Microsoft 365 aplikasi "Kami tidak dapat menyambungkan saat ini"

Jika Anda menerima pesan ini, cobalah hal berikut:

1. Periksa pengaturan firewall, perangkat lunak antivirus, dan proksi untuk mengonfirmasi bahwa firewall dan proksi tidak memblokir akses Internet Microsoft 365 lain. Lihat [URL dan rentang alamat IP Microsoft.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Buka **Mulai**  >  **Jalankan**, lalu ketik **services.msc**. Pastikan semua layanan berikut ini berjalan:
    - Penyetelan Otomatis Perangkat Tersambung Jaringan
    - Layanan Daftar Jaringan
    - Kesadaran Lokasi Jaringan
    - Windows Log Kejadian

Jika salah satu layanan ini tidak berjalan, cobalah memulainya. Jika mengalami masalah saat memulai layanan, jalankan perintah berikut dengan membuka prompt perintah dengan izin yang ditingkatkan:

**sfc /scannow**

Setelah perintah ini selesai, mulai ulang komputer.

Untuk informasi selengkapnya, lihat ["Maaf, kami tidak bisa tersambung ke akun Anda. Coba lagi nanti" saat Anda mengaktifkan Office dari Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).