---
title: Masalah dengan Pustaka Autentikasi
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004333"
- "7731"
ms.openlocfilehash: 39336fa8840a28befcad449d0afa59c1df5c6bef5988cb197916a03aa2aa66c9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028007"
---
# <a name="issues-with-authentication-libraries"></a>Masalah dengan Pustaka Autentikasi

1. [platform identitas Microsoft autentikasi mencantumkan](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) pustaka klien dan middleware yang didukung dan kompatibel dari Microsoft.
2. Pustaka Autentikasi Microsoft (MSAL, Microsoft Authentication Library) mendukung [beberapa alur autentikasi](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) untuk digunakan dalam skenario aplikasi berbeda.
3. Untuk mengautentikasi dan memperoleh token, Anda memulai aplikasi klien publik atau rahasia baru dalam kode Anda. Anda bisa mengatur beberapa opsi konfigurasi saat Anda memulai aplikasi klien di Pustaka Autentikasi Microsoft (MSAL). Untuk mempelajari selengkapnya, lihat [Opsi konfigurasi aplikasi](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).

**Akhir dukungan untuk Azure Active Directory Authentication Library (ADAL) dan API Azure AD Graph (AAD Graph)**

**Mulai 30 Juni 2020,** kami tidak akan lagi menambahkan fitur baru untuk ADAL dan Azure AD Graph. Kami akan terus menyediakan dukungan teknis dan pembaruan keamanan, namun tidak akan lagi menyediakan pembaruan fitur.

**Mulai 30 Juni 2022,** kami akan mengakhiri dukungan untuk ADAL dan Azure AD Graph dan tidak akan lagi menyediakan dukungan teknis atau pembaruan keamanan.

Aplikasi yang menggunakan ADAL di versi OS yang sudah ada akan terus berfungsi setelah saat ini, tetapi tidak akan *mendapatkan dukungan teknis atau pembaruan keamanan.*

Aplikasi yang menggunakan Azure AD Graph setelah waktu ini mungkin tidak lagi menerima respons dari titik akhir Azure AD Graph akhir.

**Migrasi ADAL**

Kami merekomendasikan Anda memperbarui ke [Pustaka Autentikasi Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), yang memiliki fitur dan pembaruan keamanan terbaru.

Jika Anda menggunakan aplikasi Microsoft, ketahui bahwa Microsoft sedang dalam proses migrasi aplikasinya ke MSAL hingga tenggat waktu akhir dukungan, yang memastikan mereka akan mendapatkan manfaat dari penyempurnaan fitur dan keamanan MSAL yang sedang berlangsung.

Untuk informasi selengkapnya, lihat:

1. [Baca FAQ ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Pelajari tentang cara melakukan migrasi aplikasi pada basis per platform](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Jika memerlukan bantuan memahami aplikasi mana yang menggunakan ADAL, kami menyarankan Anda meninjau semua kode sumber aplikasi, dan jika ada, hubungi ISVs atau penyedia aplikasi. Dukungan Microsoft juga dapat menyediakan daftar semua aplikasi non-Microsoft ADAL di penyewa Anda.

**Migrasi Grafik AAD**

Untuk aplikasi yang menggunakan Azure AD Graph, ikuti panduan kami untuk melakukan migrasi aplikasi [Azure AD Graph ke Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).

1. [Daftar periksa migrasi kami menyediakan titik mulai.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Portal pendaftaran aplikasi Azure Anda memperlihatkan aplikasi mana yang menggunakan Grafik AAD. Kami menyarankan Anda meninjau semua kode sumber aplikasi, dan jika memungkinkan, hubungi semua ISV atau penyedia aplikasi. Dukungan Microsoft juga dapat menyediakan daftar semua penggunaan AAD Graph penyewa Anda.
3. Agar aplikasi Anda mengakses data di Microsoft Graph, pengguna atau administrator harus memberikan izin yang tepat melalui proses persetujuan. Referensi [izin Graph Microsoft](https://docs.microsoft.com/graph/permissions-reference) mencantumkan izin yang terkait dengan setiap rangkaian utama API Microsoft Graph. Panduan juga tentang cara menggunakan izin.
