---
title: Bekerja dengan pustaka autentikasi
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035829"
---
# <a name="working-with-authentication-libraries"></a>Bekerja dengan pustaka autentikasi

Untuk mengatasi masalah Microsoft Authentication Library (MSAL), lakukan langkah-langkah berikut ini:

1. **Bekerja dengan MSAL**: [pustaka autentikasi platform Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) -artikel ini memperlihatkan dukungan pustaka autentikasi Microsoft untuk beberapa tipe aplikasi. Ini menyertakan link ke kode sumber pustaka; tempat untuk mendapatkan paket untuk proyek aplikasi Anda; dan apakah pustaka mendukung masuk pengguna (autentikasi), akses ke api web yang diproteksi (otorisasi), atau keduanya.

2. **Pemecahan masalah autentikasi**: msal mendukung beberapa aliran autentikasi untuk digunakan dalam skenario aplikasi yang berbeda. Tergantung pada bagaimana aplikasi klien Anda dibangun, MSAL bisa menggunakan satu atau beberapa aliran autentikasi yang didukung oleh platform Microsoft Identity. Aliran ini dapat menghasilkan beberapa tipe token dan kode otorisasi, serta memerlukan token berbeda untuk membuatnya berfungsi.

3. **Token Access**: [token akses platform Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) -Pelajari cara api Anda bisa memvalidasi dan gunakan klaim di dalam token Access. Semua dokumentasi dalam artikel ini, kecuali yang disebutkan, berlaku hanya untuk Token yang diterbitkan untuk api yang telah Anda daftarkan. Tidak berlaku untuk Token yang dikeluarkan untuk api milik Microsoft, atau token tersebut tidak dapat digunakan untuk memvalidasi bagaimana platform identitas Microsoft akan menerbitkan token untuk API yang Anda buat.

**Akhir dukungan untuk Azure Active Directory Authentication Library (ADAL)**

- **Mulai 30 juni 2020,** kami tidak akan lagi menambahkan fitur baru untuk ADAL dan Azure AD graph. Kami akan terus menyediakan dukungan teknis dan pembaruan keamanan, namun tidak akan lagi menyediakan pembaruan fitur.
- **Mulai 30 juni 2022,** kami akan mengakhiri dukungan untuk ADAL dan Azure AD graph dan tidak akan lagi menyediakan dukungan teknis atau pembaruan keamanan.
- Aplikasi yang menggunakan ADAL pada versi OS yang sudah ada akan terus berfungsi setelah waktu ini tetapi tidak akan *mendapatkan dukungan teknis atau pembaruan keamanan apa pun*.
- Aplikasi menggunakan grafik Azure AD setelah waktu ini mungkin tidak lagi menerima respons dari titik akhir Azure AD graph.

**Migrasi ADAL**

- Kami merekomendasikan memperbarui ke MSAL, yang memiliki fitur dan pembaruan keamanan terbaru.
- Jika Anda menggunakan Microsoft Apps, Ketahuilah bahwa Microsoft sedang dalam proses migrasi aplikasinya ke MSAL dengan tenggat waktu dukungan akhir, memastikan mereka akan mendapatkan manfaat dari peningkatan keamanan dan fitur yang sedang berlangsung.

1. [Baca FAQ ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
2. [Pelajari tentang cara melakukan migrasi aplikasi secara per platform](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).
3. Jika, setelah membaca panduan untuk platform aplikasi Anda, Anda memiliki pertanyaan tambahan, Anda bisa memposting di [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) dengan tag [Azure-AD-adal-bantahan] atau membuka masalah dalam repositori GitHub pustaka. Lihat bagian [bahasa dan kerangka](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) dari artikel **ringkasan msal** untuk link ke repo pustaka.
4. **Jika Anda memerlukan bantuan memahami aplikasi mana yang menggunakan ADAL**, kami menyarankan agar Anda meninjau semua kode sumber aplikasi Anda. Jika ada, hubungi vendor perangkat lunak independen (ISVs) atau penyedia aplikasi. Dukungan Microsoft juga dapat menyediakan daftar semua aplikasi non-Microsoft ADAL di penyewa Anda.







