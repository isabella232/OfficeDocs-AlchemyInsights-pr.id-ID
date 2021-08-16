---
title: Masalah dengan mengintegrasikan SSO Mulus dengan aplikasi lokal saya
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 6b295f3272ba074eac3afb66f3156af7ea4065a1398a215bcb3cde5da74b198a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028295"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Masalah dengan mengintegrasikan SSO Mulus dengan aplikasi lokal saya

Untuk memecahkan masalah dengan mengintegrasikan SSO Mulus dengan aplikasi lokal, lakukan hal berikut:

**Langkah-langkah yang direkomendasikan**

1. Untuk mengonfigurasi aplikasi lokal untuk masuk **tunggal** melalui Proksi Aplikasi, lihat Penyimpanan kata sandi untuk masuk tunggal dengan [Proksi Aplikasi.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
1. **Pemecahan masalah Proksi** Aplikasi: kami menyarankan agar Anda mulai meninjau aliran pemecahan masalah, [masalah Debug](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)Konektor Proksi Aplikasi, untuk menentukan apakah konektor Proksi Aplikasi telah dikonfigurasi dengan benar. Jika Anda masih mengalami masalah dalam menyambungkan ke aplikasi, ikuti langkah pemecahan masalah dalam [Masalah aplikasi Proksi Aplikasi Debug.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Anda dapat [mengidentifikasi masalah CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) dengan menggunakan alat debug browser berikut ini:
    1. Luncurkan browser dan telusuri ke aplikasi web.
    1. Tekan **F12** untuk memunculkan konsol debug.
    1. Cobalah untuk mereproduksi transaksi, dan tinjau pesan konsol. Pelanggaran CORS menghasilkan kesalahan konsol tentang origin.
    1. Beberapa masalah CORS tidak dapat diatasi, seperti saat aplikasi Anda mengalihkan login.microsoftonline.com ke autentikasi, dan token akses kedaluwarsa. Panggilan CORS gagal. Solusi untuk skenario ini adalah untuk memperpanjang masa berlaku token akses, untuk mencegahnya kedaluwarsa selama sesi pengguna. Untuk informasi selengkapnya tentang cara melakukan hal ini, lihat [Masa berlaku token yang dapat platform identitas Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

**Dokumen yang disarankan**

- [Cara mengonfigurasi masuk tunggal ke aplikasi Proksi Aplikasi](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [Akses masuk tunggal SAML untuk aplikasi lokal dengan Proksi Aplikasi](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Memahami dan menyelesaikan Azure Active Directory CORS Proksi Aplikasi](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Memecahkan masalah konfigurasi delegasi kerberos terbatas untuk Proksi Aplikasi](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)