---
title: Masalah mengembangkan aplikasi
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
ms.openlocfilehash: 065ff6d965063e44c4d1771821985058c9d020fbbabb0d381f30b6a11132c4ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013427"
---
# <a name="issues-developing-applications"></a>Masalah mengembangkan aplikasi

Untuk memecahkan masalah paling umum ketika menggunakan Azure Active Directory (AD), lihat artikel berikut ini:

- [Saya mengalami masalah saat masuk ke aplikasi hanya menggunakan browser Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Saya tidak tahu cara mengubah default masa berlaku token untuk aplikasi saya](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Saya bingung tentang cara kerja persetujuan aplikasi](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Saya tidak tahu cara memberikan izin untuk aplikasi saya](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Saya tidak memahami perbedaan antara izin aplikasi dan delegasi](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Akhir dukungan untuk Azure Active Directory Authentication Library (ADAL) dan API Azure AD Graph (AAD Graph)***

- Mulai tanggal 30 Juni 2020, kami tidak akan lagi menambahkan fitur baru ke Pustaka Autentikasi Azure Active Directory (ADAL) dan API Grafik Azure AD (Grafik AAD). Kami akan terus menyediakan dukungan teknis dan pembaruan keamanan, namun tidak akan lagi menyediakan pembaruan fitur.

- Mulai tanggal 30 Juni 2022, kami akan mengakhiri dukungan untuk ADAL dan Grafik AAD dan tidak akan lagi menyediakan dukungan teknis atau pembaruan keamanan. Sebagai akibat dari kondisi ini, berikut ini merupakan implikasinya:

    - Aplikasi yang menggunakan ADAL di versi OS yang sudah ada akan terus berfungsi setelah waktu ini, tetapi tidak akan mendapatkan dukungan teknis atau pembaruan keamanan apa pun.

    - Aplikasi yang menggunakan AAD Graph setelah waktu ini mungkin tidak lagi menerima respons dari titik akhir Graph AAD

**Migrasi ADAL**

Jika Anda menggunakan aplikasi Microsoft, kami menyarankan Anda memperbarui ke Pustaka Autentikasi Microsoft (MSAL, Microsoft Authentication Library), yang memiliki fitur dan pembaruan keamanan terbaru. Rekomendasi ini berada dalam konteks Microsoft memulai proses migrasi aplikasinya ke MSAL hingga tenggat waktu akhir dukungan. 

Migrasi oleh Microsoft tentang aplikasinya ke MSAL memastikan bahwa aplikasi akan mendapatkan manfaat dari keamanan berkelanjutan MSAL dan penyempurnaan fitur.

1. [Baca FAQ ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Pelajari tentang cara melakukan migrasi aplikasi pada basis per platform](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Jika memerlukan bantuan dalam memahami aplikasi mana yang menggunakan ADAL, kami menyarankan Anda meninjau semua kode sumber aplikasi, dan, jika ada, hubungi vendor perangkat lunak independen (ISVs) atau penyedia aplikasi. Dukungan Microsoft juga dapat menyediakan daftar semua aplikasi non-Microsoft ADAL di penyewa Anda.

**Migrasi Grafik AAD**

Untuk aplikasi yang menggunakan Graph AAD, ikuti panduan untuk melakukan migrasi aplikasi Graph AAD ke Microsoft Graph:

1. [Daftar periksa migrasi kami menyediakan poin memulai](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. Portal pendaftaran aplikasi Azure Anda memperlihatkan aplikasi mana yang menggunakan Grafik AAD. Kami menyarankan Anda meninjau semua kode sumber aplikasi dan, jika ada, menghubungi vendor perangkat lunak independen (ISVs) atau penyedia aplikasi. Dukungan Microsoft juga dapat menyediakan informasi tentang AAD Graph penyewa Anda.







