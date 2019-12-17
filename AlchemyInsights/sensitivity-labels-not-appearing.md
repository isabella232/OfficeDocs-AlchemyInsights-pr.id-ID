---
title: Label sensitivitas tidak muncul
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 67719380aea0481f96c03fa591542e8e5a6e6993
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048655"
---
# <a name="sensitivity-labels-not-appearing"></a>Label sensitivitas tidak muncul

Label sensitivitas memungkinkan Anda untuk mengklasifikasikan dan membantu melindungi konten sensitif Anda. Mereka dapat dibuat di Microsoft 365 kepatuhan pusat, Microsoft 365 pusat keamanan, atau Office 365 keamanan & Compliance Center di bawah klasifikasi > sensitivitas label. Untuk mempelajari lebih lanjut tentang fitur ini, lihat [Ikhtisar label sensitivitas](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels).

Jika Anda mengonfigurasi label sensitivitas namun tidak muncul di aplikasi Office, periksa hal berikut:

- Konfirmasikan bahwa label sensitivitas telah [dipublikasikan](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) ke pengguna dan grup yang Anda inginkan.

- Konfirmasikan bahwa pengguna menggunakan aplikasi yang mendukung label sensitivitas-Lihat [label sensitivitas di dokumen Anda](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?ad=US&ui=en-US&rs=en-US#bkmk_whereavailable).

- Jika Anda [memigrasi label perlindungan informasi Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), perhatikan pertimbangan yang tercantum [di sini](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).

- Dukungan pencegahan kehilangan data (DLP): saat ini, hanya label penyimpanan yang dapat digunakan sebagai kondisi dalam kebijakan DLP.  Dukungan untuk label sensitivitas dalam kebijakan DLP ini belum tersedia tapi kami sedang mengerjakannya.

- Bila enkripsi diaktifkan pada label sensitivitas, Anda dapat memilih untuk:
    - Menetapkan izin sekarang
    - Mengizinkan pengguna menetapkan izin


Untuk informasi lebih lanjut tentang kemungkinan masalah, lihat [masalah yang diketahui dengan label sensitivitas](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).