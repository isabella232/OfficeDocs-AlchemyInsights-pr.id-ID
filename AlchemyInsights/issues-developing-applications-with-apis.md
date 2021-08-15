---
title: Masalah dalam mengembangkan aplikasi dengan API
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 1de4e9aa5078507eecdbe53366e446e733029ecb1342f20ca701fa7f95a06fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013463"
---
# <a name="issues-developing-applications-with-apis"></a>Masalah dalam mengembangkan aplikasi dengan API

Untuk mulai menggunakan API Azure Active Directory Graph, lihat panduan mulai cepat [API Azure AD Graph,](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) atau lihat dokumentasi referensi [API Graph Azure AD interaktif.](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)

**Akhir dukungan untuk Azure Active Directory Authentication Library (ADAL) dan API Azure AD Graph (AAD Graph)**

**Mulai 30 Juni 2020,** kami tidak akan lagi menambahkan fitur baru untuk ADAL dan Azure AD Graph. Kami akan terus menyediakan dukungan teknis dan pembaruan keamanan, namun tidak akan lagi menyediakan pembaruan fitur.

**Mulai 30 Juni 2022,** kami akan mengakhiri dukungan untuk ADAL dan Azure AD Graph dan tidak akan lagi menyediakan dukungan teknis atau pembaruan keamanan.

Aplikasi yang menggunakan ADAL di versi OS yang sudah ada akan terus berfungsi setelah waktu ini, tetapi tidak akan mendapatkan dukungan teknis atau pembaruan keamanan apa pun.

Aplikasi yang menggunakan Azure AD Graph setelah waktu ini mungkin tidak lagi menerima respons dari titik akhir Azure AD Graph akhir.

**Migrasi ADAL**

Kami merekomendasikan Anda memperbarui ke [Pustaka Autentikasi Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), yang memiliki fitur dan pembaruan keamanan terbaru.

Jika Anda menggunakan aplikasi Microsoft, ketahui bahwa Microsoft sedang dalam proses migrasi aplikasinya ke MSAL sebelum tenggat waktu akhir dukungan, yang memastikan mereka akan mendapatkan manfaat dari keamanan msAL yang sedang berlangsung dan penyempurnaan fitur.

1. [Baca FAQ ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. [Pelajari cara melakukan migrasi aplikasi secara per platform.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. Jika memerlukan bantuan memahami aplikasi mana yang menggunakan ADAL, kami menyarankan Anda meninjau semua kode sumber aplikasi, dan jika ada, hubungi ISVs atau penyedia aplikasi. Dukungan Microsoft juga dapat menyediakan daftar semua aplikasi non-Microsoft ADAL di penyewa Anda.

**Migrasi Grafik AAD**

Untuk aplikasi yang menggunakan Azure AD Graph, ikuti panduan kami untuk melakukan migrasi aplikasi [Azure AD Graph ke Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).

1. [Daftar periksa migrasi kami menyediakan poin memulai](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. Portal pendaftaran aplikasi Azure Anda memperlihatkan aplikasi mana yang menggunakan Grafik AAD. Kami menyarankan Anda meninjau semua kode sumber aplikasi, dan jika memungkinkan, hubungi semua ISV atau penyedia aplikasi. Dukungan Microsoft juga dapat menyediakan daftar semua penggunaan AAD Graph penyewa Anda.
1. Agar aplikasi Anda mengakses data di Microsoft Graph, pengguna atau administrator harus memberikan izin yang tepat melalui proses persetujuan. Referensi [izin Graph Microsoft](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) mencantumkan izin yang terkait dengan setiap rangkaian utama API Microsoft Graph. Panduan juga tentang cara menggunakan izin.
