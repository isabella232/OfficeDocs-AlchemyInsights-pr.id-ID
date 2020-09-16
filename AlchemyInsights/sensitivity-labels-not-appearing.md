---
title: Label sensitivitas tidak muncul
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 6a64e001be115c8e5553a0d8c97b8cb815922c69
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801187"
---
# <a name="sensitivity-labels-not-appearing"></a>Label sensitivitas tidak muncul

Label sensitivitas memungkinkan Anda mengelompokkan dan membantu melindungi konten sensitif Anda. Mereka dapat dibuat di pusat kepatuhan Microsoft 365, Pusat Keamanan Microsoft 365, atau Microsoft 365 Security & Compliance Center di bawah klasifikasi > label sensitivitas. Untuk mempelajari selengkapnya tentang fitur ini, lihat [gambaran umum label sensitivitas](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).

Jika Anda mengonfigurasi label sensitivitas tetapi tidak muncul di aplikasi Microsoft 365, periksa hal berikut ini:

- Konfirmasi bahwa label sensitivitas telah [diterbitkan](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) untuk pengguna dan grup yang Anda inginkan.

- Konfirmasi bahwa pengguna menggunakan aplikasi yang mendukung label sensitivitas-Lihat [label sensitivitas dalam dokumen Anda](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).

- Jika Anda melakukan [migrasi label proteksi informasi Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), perhatikan pertimbangan yang tercantum [di sini](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).

- Dukungan pencegahan kehilangan data (DLP): saat ini, hanya label penyimpanan yang dapat digunakan sebagai kondisi dalam kebijakan DLP.  Dukungan untuk label sensitivitas dalam kebijakan DLP belum tersedia tetapi kami sedang mengerjakannya.

- Saat enkripsi diaktifkan pada label sensitivitas, Anda bisa memilih untuk:
    - Tetapkan izin sekarang
    - Memungkinkan pengguna memberikan izin


Untuk informasi selengkapnya tentang masalah yang mungkin terjadi, lihat [masalah yang diketahui dengan label sensitivitas](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).