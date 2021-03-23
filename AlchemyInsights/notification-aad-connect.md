---
title: Koneksi AAD pemberitahuan
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
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036109"
---
# <a name="notification-aad-connect"></a>Koneksi AAD pemberitahuan

- Pastikan Anda memiliki wewenang untuk melakukan operasi. Admin global memiliki akses secara default. Selain itu, Anda bisa menggunakan [kontrol akses berbasis peran](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) untuk mendelegasikan izin pendaftaran ke kontributor.
- Pastikan titik akhir yang diperlukan diaktifkan, dan tidak diblokir karena firewall. Untuk detailnya, lihat [persyaratan](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Pendaftaran dapat gagal karena komunikasi keluar menjadi sasaran inspeksi SSL oleh lapisan jaringan.
- Pastikan Anda telah memverifikasi pengaturan pemberitahuan untuk kesehatan Azure AD Connect dan Tinjau pengaturan Anda. Untuk memahami cara mengonfigurasi pengaturan pemberitahuan untuk pemberitahuan kesehatan Azure AD Connect, lihat [panduan](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)ini.
- Untuk mempelajari selengkapnya tentang laporan sinkronisasi kesehatan AAD Connect dan cara mengunduhnya, lihat [laporan tingkat objek sinkronisasi](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

Untuk memecahkan masalah pemberitahuan kesehatan AAD Connect ikuti [panduan pemecahan masalah untuk data kesehatan pemberitahuan KESEGARAN AAD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) dan untuk tanya umum, lihat [pertanyaan umum penginstalan kesehatan AAD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).
