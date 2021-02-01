---
title: Masalah dengan pustaka autentikasi
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
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063636"
---
# <a name="issues-with-authentication-libraries"></a>Masalah dengan pustaka autentikasi

1. [Pustaka autentikasi platform identitas Microsoft](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) mencantumkan pustaka klien dan middleware yang didukung Microsoft dan kompatibel.
2. Pustaka autentikasi Microsoft (MSAL) mendukung beberapa [aliran autentikasi](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) untuk digunakan dalam skenario aplikasi yang berbeda.
3. Untuk mengautentikasi dan memperoleh token, Anda menginisialisasi aplikasi klien publik atau rahasia baru di kode Anda. Anda bisa mengatur beberapa opsi konfigurasi saat Anda menginisialisasi aplikasi klien di pustaka autentikasi Microsoft (MSAL). Untuk mempelajari selengkapnya, lihat [opsi konfigurasi aplikasi](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).

**Akhir dukungan untuk Azure Active Directory Authentication Library (ADAL) dan Azure AD graph API (Graf AAD)**

**Mulai 30 juni 2020**, kami tidak akan lagi menambahkan fitur baru untuk ADAL dan Azure AD graph. Kami akan terus menyediakan dukungan teknis dan pembaruan keamanan, namun tidak akan lagi menyediakan pembaruan fitur.

**Mulai 30 juni 2022**, kami akan mengakhiri dukungan untuk ADAL dan Azure AD graph dan tidak akan lagi menyediakan dukungan teknis atau pembaruan keamanan.

Aplikasi yang menggunakan ADAL pada versi OS yang sudah ada akan terus berfungsi setelah waktu ini tetapi tidak akan *mendapatkan dukungan teknis atau pembaruan keamanan apa pun*.

Aplikasi menggunakan grafik Azure AD setelah waktu ini mungkin tidak lagi menerima respons dari titik akhir Azure AD graph.

**Migrasi ADAL**

Kami merekomendasikan Anda memperbarui ke [Pustaka Autentikasi Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), yang memiliki fitur dan pembaruan keamanan terbaru.

Jika Anda menggunakan Microsoft Apps, Ketahuilah bahwa Microsoft sedang dalam proses migrasi aplikasinya ke MSAL dengan tenggat waktu dukungan akhir, memastikan mereka akan mendapatkan manfaat dari keamanan dan penyempurnaan fitur yang sedang berlangsung.

Untuk informasi selengkapnya, lihat:

1. [Baca FAQ ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Pelajari tentang cara melakukan migrasi aplikasi pada basis per platform](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Jika Anda memerlukan bantuan untuk memahami aplikasi mana yang menggunakan ADAL, kami menyarankan agar Anda meninjau semua kode sumber aplikasi Anda, dan jika ada, hubungi penyedia ISVs atau aplikasi apa pun. Dukungan Microsoft juga dapat menyediakan daftar semua aplikasi non-Microsoft ADAL di penyewa Anda.

**Migrasi Grafik AAD**

Untuk aplikasi yang menggunakan Azure AD graph, ikuti panduan kami untuk melakukan [migrasi aplikasi AZURE AD graph ke Microsoft graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).

1. [Daftar Periksa migrasi kami menyediakan titik mulai.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Portal pendaftaran aplikasi Azure Anda memperlihatkan aplikasi mana yang menggunakan Grafik AAD. Kami menyarankan Anda meninjau semua kode sumber aplikasi, dan jika memungkinkan, hubungi semua ISV atau penyedia aplikasi. Dukungan Microsoft juga bisa memberi Anda daftar semua penggunaan grafik AAD dalam penyewa Anda.
3. Agar aplikasi Anda dapat mengakses data di Microsoft graph, pengguna atau administrator harus memberinya izin yang benar melalui proses persetujuan. [Referensi izin Microsoft graph](https://docs.microsoft.com/graph/permissions-reference) mencantumkan izin yang terkait dengan setiap kumpulan utama api Microsoft graph. Ini juga memberikan panduan tentang cara menggunakan izin.
