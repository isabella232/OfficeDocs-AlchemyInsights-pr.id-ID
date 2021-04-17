---
title: Memperbaiki aplikasi Microsoft 365 Maaf, kami mengalami pesan masalah server sementara
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
- "3420"
- "9001430"
ms.openlocfilehash: 0adf1d66869051b9dd8290ef3466ef9b13aa2d41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835274"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Memperbaiki pesan "Maaf, kami mengalami masalah server sementara" aplikasi Microsoft 365

Jika Anda menerima pesan ini, cobalah hal berikut:

1. Periksa pengaturan firewall, perangkat lunak antivirus, dan proksi untuk mengonfirmasi bahwa firewall dan proksi tidak memblokir akses Internet ke aplikasi Microsoft 365. Lihat [URL dan rentang alamat IP.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Buka **Mulai**  >  **Jalankan**, lalu ketik **services.msc**. Pastikan semua layanan berikut ini berjalan:
    - Penyetelan Otomatis Perangkat Tersambung Jaringan
    - Layanan Daftar Jaringan
    - Kesadaran Lokasi Jaringan
    - Log Kejadian Windows

Jika salah satu layanan ini tidak berjalan, cobalah memulainya. Jika mengalami masalah saat memulai layanan, jalankan perintah berikut dengan membuka prompt perintah dengan izin yang ditingkatkan:

**sfc /scannow**

Setelah perintah ini selesai, mulai ulang komputer.

Untuk informasi selengkapnya, lihat ["Maaf, kami tidak bisa tersambung ke akun Anda. Coba lagi nanti" saat Anda mengaktifkan](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).