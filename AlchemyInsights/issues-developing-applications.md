---
title: Masalah dalam mengembangkan aplikasi
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974472"
---
# <a name="issues-developing-applications"></a>Masalah dalam mengembangkan aplikasi

Untuk memecahkan masalah paling umum ketika membuat aplikasi Azure Active Directory (AD), lihat artikel berikut ini:

- [Saya mengalami masalah saat masuk ke aplikasi menggunakan browser Chrome saja](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Saya tidak tahu cara mengubah default seumur hidup token untuk aplikasi saya](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Saya bingung tentang cara kerja persetujuan aplikasi](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Saya tidak tahu cara memberikan izin ke aplikasi saya](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Saya tidak memahami perbedaan antara izin delegasi dan aplikasi](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Akhir dukungan untuk Azure Active Directory Authentication Library (ADAL) dan AZURE AD GRAPH api (GRAF AAD)** _

- Mulai tanggal 30 Juni 2020, kami tidak akan lagi menambahkan fitur baru ke pustaka autentikasi direktori aktif Azure (ADAL) dan Azure AD graph API (Graf AAD). Kami akan terus menyediakan dukungan teknis dan pembaruan keamanan tetapi tidak lagi menyediakan pembaruan fitur.

- Mulai 30 Juni 2022, kami akan mengakhiri dukungan untuk Graf ADAL dan AAD dan tidak lagi menyediakan dukungan teknis atau pembaruan keamanan. Sebagai akibat dari kondisi ini, berikut ini adalah implikasi:

    - Aplikasi yang menggunakan ADAL pada versi OS yang sudah ada akan terus berfungsi setelah waktu ini tetapi tidak akan mendapatkan dukungan teknis atau pembaruan keamanan apa pun.

    - Aplikasi menggunakan grafik AAD setelah waktu ini mungkin tidak lagi menerima respons dari titik akhir Graf AAD

_ *Migrasi ADAL**

Jika Anda menggunakan aplikasi Microsoft, sebaiknya Perbarui ke Microsoft Authentication Library (MSAL), yang memiliki fitur dan pembaruan keamanan terbaru. Rekomendasi ini adalah dalam konteks Microsoft memulai proses migrasi aplikasinya ke MSAL dengan tenggat waktu dukungan akhir. 

Migrasi dengan Microsoft dari aplikasinya ke MSAL memastikan bahwa aplikasi tersebut mendapatkan manfaat dari penyempurnaan fitur dan keamanan yang sedang berlangsung.

1. [Membaca FAQ ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Pelajari tentang cara melakukan migrasi aplikasi secara per platform](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Jika Anda memerlukan bantuan dalam memahami aplikasi mana yang menggunakan ADAL, kami menyarankan agar Anda meninjau semua kode sumber aplikasi Anda dan, jika ada, menjangkau ke vendor perangkat lunak independen (ISVs) atau penyedia aplikasi. Dukungan Microsoft juga bisa memberi Anda daftar semua aplikasi non-Microsoft ADAL di penyewa Anda.

**Migrasi Graf AAD**

Untuk aplikasi yang menggunakan grafik AAD, ikuti panduan kami untuk melakukan migrasi aplikasi Graf AAD ke Microsoft graph:

1. [Daftar Periksa migrasi kami menyediakan titik mulai](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. Portal pendaftaran aplikasi Azure memperlihatkan aplikasi mana yang menggunakan grafik AAD. Kami menyarankan agar Anda meninjau semua kode sumber aplikasi dan, jika ada, menjangkau ke vendor perangkat lunak independen (ISVs) atau penyedia aplikasi. Dukungan Microsoft juga bisa memberi Anda informasi tentang penggunaan grafik AAD dalam penyewa Anda.







