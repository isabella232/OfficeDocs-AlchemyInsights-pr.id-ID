---
title: Masalah saat mengintegrasikan Seamless SSO dengan aplikasi lokal saya
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
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/13/2021
ms.locfileid: "49868714"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Masalah saat mengintegrasikan Seamless SSO dengan aplikasi lokal saya

Untuk memecahkan masalah saat mengintegrasikan SSO tanpa hambatan dengan aplikasi di tempat, lakukan hal berikut:

**Langkah yang direkomendasikan**

1. Untuk mengonfigurasi **aplikasi lokal** untuk **masuk tunggal melalui proksi aplikasi**, lihat [kubah kata sandi untuk masuk tunggal dengan proksi aplikasi](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
1. **Pemecahan masalah proksi aplikasi**: kami menyarankan agar Anda mulai meninjau alur pemecahan masalah [konektor proksi aplikasi debug](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), untuk menentukan apakah konektor proksi aplikasi dikonfigurasikan dengan benar. Jika Anda masih mengalami masalah saat menyambungkan ke aplikasi, ikuti langkah-langkah pemecahan masalah dalam [masalah aplikasi proksi aplikasi debug](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). Anda bisa [mengidentifikasi masalah CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) dengan menggunakan alat debug browser berikut ini:
    1. Luncurkan browser dan telusuri ke aplikasi web.
    1. Tekan **F12** untuk memunculkan konsol debug.
    1. Cobalah untuk mereproduksi transaksi, dan Tinjau pesan konsol. Pelanggaran CORS menghasilkan kesalahan konsol tentang Origin.
    1. Beberapa masalah CORS tidak bisa diatasi, seperti ketika aplikasi Anda mengalihkan ke login.microsoftonline.com untuk diautentikasi, dan token akses kedaluwarsa. Panggilan CORS lalu gagal. Penanganan masalah untuk skenario ini adalah memperpanjang masa berlaku token Access, untuk mencegahnya kedaluwarsa selama sesi pengguna. Untuk informasi selengkapnya tentang cara melakukannya, lihat [masa Token yang dapat dikonfigurasikan dalam platform Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

**Dokumen yang direkomendasikan**

- [Cara mengonfigurasi single sign-on ke aplikasi proksi aplikasi](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [Single sign-on SAML untuk aplikasi lokal dengan proksi aplikasi](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Memahami dan memecahkan masalah CORS proksi aplikasi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Memecahkan masalah konfigurasi delegasi Kerberos yang dibatasi untuk proksi aplikasi](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)