---
title: Masalah dengan AAD Koneksi Kesehatan
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
ms.openlocfilehash: 82cfcc6132549b52278b174fce3173f5566268864a207882a4dd639cb8024ee3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923755"
---
# <a name="problem-with-aad-connect-health"></a>Masalah dengan AAD Koneksi Kesehatan

- Pastikan Anda memiliki wewenang untuk melakukan operasi. Admin Global secara default memiliki akses. Selain itu, Anda bisa menggunakan [Kontrol Akses Berbasis Peran](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) untuk mendelegasikan izin pendaftaran ke Kontributor.
- Pastikan titik akhir yang diperlukan diaktifkan, dan tidak diblokir karena firewall. Untuk detailnya, lihat [persyaratan](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Pendaftaran dapat gagal karena komunikasi keluar sedang dikenakan inspeksi SSL oleh lapisan jaringan.
- Pastikan Anda telah memverifikasi pengaturan pemberitahuan untuk Azure AD Koneksi Health. Silakan tinjau pengaturan Anda. Panduan [ini](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) dapat membantu Anda memahami cara mengonfigurasi pengaturan pemberitahuan untuk Azure AD Koneksi pemberitahuan kesehatan.
- Untuk mempelajari selengkapnya tentang laporan sinkronisasi AAD Koneksi Kesehatan dan cara mengunduhnya, lihat [Laporan sinkronisasi tingkat objek](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

Untuk memecahkan masalah Koneksi AAD, ikuti panduan pemecahan masalah untuk pemberitahuan [pembaruan data AAD Koneksi](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) Kesehatan dan untuk pertanyaan yang sering diajukan, lihat Pertanyaan umum penginstalan [AAD Koneksi Kesehatan.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)
