---
title: Masalah dengan AAD Connect Health
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482069"
---
# <a name="problem-with-aad-connect-health"></a>Masalah dengan AAD Connect Health

- Pastikan Anda memiliki wewenang untuk melakukan operasi. Admin global memiliki akses secara default. Selain itu, Anda bisa menggunakan [kontrol akses berbasis peran](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) untuk mendelegasikan izin pendaftaran ke kontributor.
- Pastikan titik akhir yang diperlukan diaktifkan, dan tidak diblokir karena firewall. Untuk detailnya, lihat [persyaratan](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Pendaftaran dapat gagal karena komunikasi keluar menjadi sasaran inspeksi SSL oleh lapisan jaringan.
- Pastikan Anda telah memverifikasi pengaturan pemberitahuan untuk kesehatan Azure AD Connect. Tinjau pengaturan Anda. [Panduan](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) ini dapat membantu Anda memahami cara mengonfigurasi pengaturan pemberitahuan untuk pemberitahuan kesehatan Azure AD Connect.
- Untuk mempelajari selengkapnya tentang laporan sinkronisasi kesehatan AAD Connect dan cara mengunduhnya, lihat [laporan tingkat objek sinkronisasi](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

Untuk memecahkan masalah pemberitahuan kesehatan AAD Connect, ikuti [panduan pemecahan masalah untuk menyambungkan pemberitahuan kesegaran data kesehatan](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) dan tanya jawab umum, lihat [pertanyaan umum tentang penginstalan kesehatan AAD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).
