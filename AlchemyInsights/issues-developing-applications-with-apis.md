---
title: Masalah dalam mengembangkan aplikasi dengan api
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
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974621"
---
# <a name="issues-developing-applications-with-apis"></a>Masalah dalam mengembangkan aplikasi dengan api

Untuk mulai menggunakan API grafik Azure Active Directory, lihat [panduan mulai cepat AZURE AD GRAPH api](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , atau Tampilkan [dokumentasi referensi api Azure AD graph interaktif](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).

**Akhir dukungan untuk Azure Active Directory Authentication Library (ADAL) dan Azure AD graph API (Graf AAD)**

**Mulai 30 juni 2020**, kami tidak akan lagi menambahkan fitur baru untuk ADAL dan Azure AD graph. Kami akan terus menyediakan dukungan teknis dan pembaruan keamanan tetapi tidak lagi menyediakan pembaruan fitur.

**Mulai 30 juni 2022**, kami akan mengakhiri dukungan untuk ADAL dan Azure AD graph dan tidak akan lagi menyediakan dukungan teknis atau pembaruan keamanan.

Aplikasi yang menggunakan ADAL pada versi OS yang sudah ada akan terus berfungsi setelah waktu ini tetapi tidak akan mendapatkan dukungan teknis atau pembaruan keamanan apa pun.

Aplikasi menggunakan grafik Azure AD setelah waktu ini mungkin tidak lagi menerima respons dari titik akhir Azure AD graph.

**Migrasi ADAL**

Sebaiknya Perbarui ke [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), yang memiliki fitur dan pembaruan keamanan terbaru.

Jika Anda menggunakan Microsoft Apps, Ketahuilah bahwa Microsoft sedang dalam proses migrasi aplikasinya ke MSAL dengan tenggat waktu dukungan akhir, memastikan mereka akan mendapatkan manfaat dari peningkatan keamanan dan fitur yang sedang berlangsung.

1. [Baca FAQ ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. [Pelajari tentang cara melakukan migrasi aplikasi secara per platform](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. Jika Anda memerlukan bantuan untuk memahami aplikasi mana yang menggunakan ADAL, kami menyarankan agar Anda meninjau semua kode sumber aplikasi Anda, dan jika ada, hubungi penyedia ISVs atau aplikasi apa pun. Dukungan Microsoft juga bisa memberi Anda daftar semua aplikasi non-Microsoft ADAL di penyewa Anda.

**Migrasi Graf AAD**

Untuk aplikasi yang menggunakan Azure AD graph, ikuti panduan kami untuk melakukan migrasi [aplikasi AZURE AD graph ke Microsoft graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).

1. [Daftar Periksa migrasi kami menyediakan titik mulai](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. Portal pendaftaran aplikasi Azure memperlihatkan aplikasi mana yang menggunakan grafik AAD. Kami menyarankan agar Anda meninjau semua kode sumber aplikasi, dan jika ada, hubungi penyedia ISVs atau aplikasi apa pun. Dukungan Microsoft juga bisa memberi Anda daftar semua penggunaan grafik AAD dalam penyewa Anda.
1. Agar aplikasi Anda dapat mengakses data di Microsoft graph, pengguna atau administrator harus memberinya izin yang benar melalui proses persetujuan. [Referensi izin Microsoft graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) mencantumkan izin yang terkait dengan setiap kumpulan utama api Microsoft graph. Ini juga memberikan panduan tentang cara menggunakan izin.
