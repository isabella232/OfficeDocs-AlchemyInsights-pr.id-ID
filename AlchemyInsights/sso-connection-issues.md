---
title: Masalah Koneksi SSO
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
ms.openlocfilehash: 8fb93bc40c6cd5a7c0e3d259fe3be8d1bab3187dd5aa023eb49977555fd930de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084349"
---
# <a name="sso-connection-issues"></a>Masalah Koneksi SSO

1. Ikuti Mulai [Cepat: Mengonfigurasi properti untuk panduan aplikasi](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) dalam mengonfigurasi aplikasi.
2. Tergantung pada opsi aplikasi dan [Masuk tunggal yang dipilih,](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) ikuti panduan yang sesuai di bawah ini:
    - Untuk mengonfigurasi **aplikasi lokal** untuk akses masuk tunggal berbasis **SAML,** lihat Akses masuk tunggal SAML untuk aplikasi lokal dengan [Proksi Aplikasi.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
    - Untuk mengonfigurasi aplikasi **awan** untuk **akses masuk tunggal berbasis kata sandi,** lihat Mengonfigurasi akses masuk tunggal kata [sandi.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)
    - Untuk mengonfigurasi aplikasi lokal untuk masuk **tunggal** melalui Proksi Aplikasi, lihat Penyimpanan kata sandi untuk masuk tunggal dengan [Proksi Aplikasi.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
3. **Pemecahan masalah Proksi** Aplikasi: kami menyarankan Anda untuk mulai meninjau aliran pemecahan masalah, [Masalah Debug Konektor](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)Proksi Aplikasi , untuk menentukan apakah konektor Proksi Aplikasi telah dikonfigurasi dengan benar. Jika Anda masih mengalami masalah dalam menyambungkan ke aplikasi, ikuti alur pemecahan masalah dalam [Masalah aplikasi Proksi Aplikasi Debug.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Anda dapat [mengidentifikasi masalah CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) dengan menggunakan alat debug browser:
    - Luncurkan browser dan telusuri ke aplikasi web.
    - Tekan **F12** untuk memunculkan konsol debug.
    - Cobalah untuk mereproduksi transaksi, dan tinjau pesan konsol. Pelanggaran CORS menghasilkan kesalahan konsol tentang origin.
    - Beberapa masalah CORS tidak dapat diatasi, seperti saat aplikasi Anda mengalihkan login.microsoft.com ke autentikasi, dan token akses kedaluwarsa. Panggilan CORS gagal. Solusi untuk skenario ini adalah untuk memperpanjang masa berlaku token akses, untuk mencegahnya kedaluwarsa selama sesi pengguna. Untuk informasi selengkapnya tentang cara melakukan hal ini, lihat [Masa berlaku token yang dapat platform identitas Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
4. Pemecahan masalah akses masuk tunggal berbasis **SAML:** kami menyarankan Anda memeriksa Masalah masuk ke aplikasi akses masuk tunggal berbasis [SAML,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)untuk menemukan solusi untuk masalah yang kemungkinan besar Anda alami.
5. **Pemecahan masalah akses** masuk tunggal berbasis kata sandi: kami menyarankan Anda memeriksa Pecahkan masalah akses masuk tunggal berbasis kata sandi di [Azure AD,](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)untuk menemukan solusi untuk masalah yang paling sering ditemui.
6. Untuk masalah koneksi saat menggunakan VPN, [lihat Cara menggunakan masuk tunggal (SSO) melalui VPN Wi-Fi koneksi](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections).
