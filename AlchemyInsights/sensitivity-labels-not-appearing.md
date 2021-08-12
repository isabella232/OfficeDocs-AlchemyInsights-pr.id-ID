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
ms.openlocfilehash: 824824257fee4aaaab1f2dd32597b4cdc858d035fabd357af90cf054dd35c9c4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061435"
---
# <a name="sensitivity-labels-not-appearing"></a>Label sensitivitas tidak muncul

Label sensitivitas memungkinkan Anda mengklasifikasikan dan membantu melindungi konten sensitif Anda. Aplikasi dapat dibuat di pusat keamanan pusat kepatuhan Microsoft 365, Microsoft 365, atau Microsoft 365 keamanan & di bawah Klasifikasi > Label Sensitivitas. Untuk mempelajari selengkapnya tentang fitur ini, lihat [Gambaran umum label sensitivitas](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).

Jika Anda mengonfigurasi label sensitivitas Anda tapi label tersebut tidak muncul di aplikasi Microsoft 365, periksa hal berikut ini:

- Konfirmasi bahwa label sensitivitas telah [diterbitkan ke](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) pengguna dan grup yang Anda inginkan.

- Pastikan bahwa pengguna menggunakan aplikasi yang mendukung label sensitivitas , lihat [label sensitivitas di dokumen Anda](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).

- Jika Anda melakukan [migrasi label Perlindungan Informasi Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), ketahuilah pertimbangan yang tercantum di [sini.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)

- Dukungan Pencegahan kehilangan data (DLP): Saat ini, hanya label penyimpanan yang bisa digunakan sebagai kondisi dalam kebijakan DLP.  Dukungan untuk label sensitivitas dalam kebijakan DLP belum tersedia tapi kami sedang mengerjakannya.

- Ketika enkripsi diaktifkan pada label sensitivitas, Anda dapat memilih salah satu untuk:
    - Tetapkan izin sekarang
    - Izinkan pengguna menetapkan izin


Untuk informasi selengkapnya tentang masalah yang mungkin terjadi, lihat [Masalah umum dengan label sensitivitas](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).