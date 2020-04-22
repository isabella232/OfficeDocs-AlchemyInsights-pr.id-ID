---
title: Memperbaiki aplikasi Office Maaf, kami mengalami pesan masalah server sementara
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
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764120"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a>Memperbaiki aplikasi Office "Maaf, kami mengalami masalah server sementara" pesan

Jika Anda menerima pesan ini, cobalah berikut ini:

1. Periksa firewall, perangkat lunak antivirus, dan pengaturan proxy untuk mengonfirmasi bahwa mereka tidak memblokir akses internet ke aplikasi Office. Lihat [rentang URL dan alamat IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Pergi ke **mulai** > **menjalankan**, dan kemudian ketik **Services. MSC**. Pastikan bahwa layanan berikut ini berjalan:
    - Jaringan tersambung perangkat Auto-setup
    - Layanan daftar jaringan
    - Kesadaran lokasi jaringan
    - Log peristiwa Windows

Jika salah satu layanan ini tidak berjalan, cobalah untuk memulainya. Jika Anda memiliki masalah memulai layanan, jalankan perintah berikut ini dengan membuka prompt perintah dengan izin yang ditinggikan:

**SFC/SCANNOW**

Setelah perintah ini selesai, mulai ulang komputer.

Untuk informasi terperinci, lihat ["Maaf, kami tidak dapat tersambung ke akun Anda. Silakan coba lagi nanti "galat saat Anda mengaktifkan](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).