---
title: Memperbaiki aplikasi Microsoft 365 Maaf, kami mengalami pesan masalah server sementara
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582706"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Memperbaiki aplikasi Microsoft 365 "Maaf, kami mengalami masalah server sementara" pesan

Jika Anda menerima pesan ini, cobalah berikut ini:

1. Periksa firewall, perangkat lunak antivirus, dan pengaturan proxy untuk mengonfirmasi bahwa mereka tidak memblokir akses internet ke aplikasi Microsoft 365. Lihat [rentang URL dan alamat IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Pergi ke **mulai**  >  **menjalankan**, dan kemudian ketik **Services. MSC**. Pastikan bahwa layanan berikut ini berjalan:
    - Jaringan tersambung perangkat Auto-setup
    - Layanan daftar jaringan
    - Kesadaran lokasi jaringan
    - Log peristiwa Windows

Jika salah satu layanan ini tidak berjalan, cobalah untuk memulainya. Jika Anda memiliki masalah memulai layanan, jalankan perintah berikut ini dengan membuka prompt perintah dengan izin yang ditinggikan:

**SFC/SCANNOW**

Setelah perintah ini selesai, mulai ulang komputer.

Untuk informasi terperinci, lihat ["Maaf, kami tidak dapat tersambung ke akun Anda. Silakan coba lagi nanti "galat saat Anda mengaktifkan](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).