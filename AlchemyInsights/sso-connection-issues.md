---
title: Masalah koneksi SSO
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
- "9004357"
- "7810"
ms.openlocfilehash: 33074d70377866332feeccfb8b6400eff2de5a73
ms.sourcegitcommit: e188ec7a583837a3e07880d05b3607b8bdac729c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935150"
---
# <a name="sso-connection-issues"></a>Masalah koneksi SSO

1. Ikuti [mulai cepat: mengonfigurasi properti untuk panduan aplikasi](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) guna mengonfigurasi aplikasi Anda.
2. Bergantung pada [opsi masuk tunggal](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) dan aplikasi yang Anda pilih, ikuti panduan yang sesuai di bawah ini:
    - Untuk mengonfigurasi **aplikasi lokal** untuk **masuk tunggal berbasis SAML**, lihat [single sign-on SAML untuk aplikasi lokal dengan proksi aplikasi](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps).
    - Untuk mengonfigurasi **aplikasi awan** untuk **masuk tunggal berbasis kata sandi**, lihat  [mengonfigurasi akses masuk tunggal kata sandi](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications).
    - Untuk mengonfigurasi **aplikasi lokal** untuk **masuk tunggal melalui proksi aplikasi**, lihat [kubah kata sandi untuk masuk tunggal dengan proksi aplikasi](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
3. **Pemecahan masalah proksi aplikasi**: kami menyarankan agar Anda mulai meninjau alur pemecahan masalah [konektor proksi aplikasi debug](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), untuk menentukan apakah konektor proksi aplikasi dikonfigurasikan dengan benar. Jika Anda masih mengalami masalah saat menyambungkan ke aplikasi, ikuti masalah alur pemecahan masalah dalam aplikasi [proksi aplikasi debug](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). Anda bisa [mengidentifikasi masalah CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) dengan menggunakan alat debug browser:
    - Luncurkan browser dan telusuri ke aplikasi web.
    - Tekan **F12** untuk memunculkan konsol debug.
    - Cobalah untuk mereproduksi transaksi, dan Tinjau pesan konsol. Pelanggaran CORS menghasilkan kesalahan konsol tentang Origin.
    - Beberapa masalah CORS tidak bisa diatasi, seperti ketika aplikasi Anda mengalihkan ke login.microsoft.com untuk diautentikasi, dan token akses kedaluwarsa. Panggilan CORS lalu gagal. Penanganan masalah untuk skenario ini adalah memperpanjang masa berlaku token Access, untuk mencegahnya kedaluwarsa selama sesi pengguna. Untuk informasi selengkapnya tentang cara melakukannya, lihat [masa Token yang dapat dikonfigurasikan dalam platform Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
4. **Pemecahan masalah masuk tunggal berbasis SAML**: kami menyarankan Anda memeriksa [masalah masuk ke aplikasi tunggal berbasis SAML yang dikonfigurasikan](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery), untuk menemukan solusi untuk masalah yang mungkin Anda temui.
5. **Pemecahan masalah akses menyeluruh berbasis kata sandi**: kami menyarankan Anda memeriksa [pemecahan masalah masuk tunggal berbasis kata sandi di Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso), untuk menemukan solusi untuk masalah yang mungkin Anda temui.
6. Untuk masalah koneksi saat menggunakan VPN, lihat [cara menggunakan masuk tunggal (SSO) melalui vpn dan koneksi Wi-Fi](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections).
