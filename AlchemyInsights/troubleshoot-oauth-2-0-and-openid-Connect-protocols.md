---
title: Memecahkan masalah protokol OAuth 2,0 dan OpenID Connect
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
- "9776"
- "9004342"
ms.openlocfilehash: d2f14d4d16bea890b564cdb9bd9ac3875c28d115
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036405"
---
# <a name="troubleshoot-oauth-20-and-openid-connect-protocols"></a>Memecahkan masalah protokol OAuth 2,0 dan OpenID Connect

Untuk mengatasi masalah OAuth 2,0 dan OpenID Connect, lakukan langkah-langkah berikut ini:

Lihat artikel berikut yang terkait dengan konfigurasi dan pemecahan masalah protokol koneksi OAuth 2,0 dan OpenID:

- [Alur kode Microsoft Identity platform dan OAuth 2,0 otorisasi](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) -artikel ini menjelaskan cara memprogram langsung terhadap **aliran Code Grant (pkce)** dalam aplikasi Anda, menggunakan bahasa apa pun.
- [Platform identitas Microsoft dan alur kredensial klien 2,0 OAuth](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) -artikel ini menguraikan cara program langsung terhadap **aliran kredensial klien** dalam aplikasi Anda.
- [Kredensial kata sandi Microsoft Identity platform dan sumber daya 2,0 OAuth](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth-ropc) -artikel ini menjelaskan cara memprogram langsung terhadap **aliran ropc** dalam aplikasi Anda.
    - Platform identitas Microsoft hanya mendukung ROPC untuk penyewa Azure AD, dan bukan untuk akun pribadi. Ini berarti bahwa Anda harus menggunakan titik akhir penyewa-spesifik **( https://login.microsoftonline.com/{TenantId_or_Name})** atau titik akhir **organisasi** .
    - Akun pribadi yang diundang ke penyewa Azure AD tidak dapat menggunakan ROPC.
    - Akun yang tidak memiliki kata sandi tidak bisa masuk melalui ROPC. Untuk skenario ini, kami menyarankan agar Anda menggunakan aliran berbeda untuk aplikasi Anda.
    - Jika pengguna perlu menggunakan [multi-Factor Authentication (MFA)](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-howitworks) untuk masuk ke aplikasi, maka mereka akan diblokir.
    - ROPC tidak didukung dalam skenario [Federasi identitas hibrid](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-fed) (misalnya, Azure AD dan ADFS yang digunakan untuk mengotentikasi akun lokal). Jika pengguna memiliki halaman penuh dialihkan ke penyedia identitas lokal, Azure AD tidak dapat menguji nama pengguna dan kata sandi terhadap penyedia identitas tersebut. [Autentikasi kirim](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta) langsung didukung dengan ropc.
    - Pengecualian untuk skenario Federasi identitas hibrid adalah sebagai berikut: kebijakan penemuan Realm rumah dengan kumpulan **pengesahan Allowcloudpassworddiatur** ke **True** akan mengaktifkan aliran ropc agar berfungsi bagi pengguna yang tergabung saat kata sandi lokal disinkronkan ke awan. Untuk informasi selengkapnya, lihat [mengaktifkan autentikasi langsung pengguna gabungan untuk aplikasi warisan](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#enable-direct-ropc-authentication-of-federated-users-for-legacy-applications) 
- [Platform identitas Microsoft dan 2,0 OAuth atas nama-aliran](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) -artikel ini menjelaskan cara memprogram secara langsung terhadap **aliran di atas nama (OBO)** dalam aplikasi Anda.
- [Microsoft Identity platform dan OpenID Connect Protocol](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) -artikel ini memperlihatkan cara menerapkan protokol OpenID Connect independen dari bahasa, dan menjelaskan cara untuk mengirim dan menerima pesan http tanpa menggunakan pustaka sumber terbuka Microsoft.

**Token Access**

[Token Access platform identitas Microsoft](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) -Pelajari bagaimana api Anda bisa memvalidasi dan menggunakan klaim di dalam token Access. Semua dokumentasi dalam artikel ini, kecuali yang disebutkan, berlaku hanya untuk Token yang diterbitkan untuk api yang telah Anda daftarkan. Tidak berlaku untuk Token yang dikeluarkan untuk api milik Microsoft, atau token tersebut tidak dapat digunakan untuk memvalidasi bagaimana platform identitas Microsoft akan menerbitkan token untuk API yang Anda buat.

**Konfigurasi aplikasi**

[Pembatasan dan pembatasan URI redirect (URL Balasan)](https://docs.microsoft.com/azure/active-directory/develop/reply-url) -Pelajari cara MENGONFIGURASI pengalihan URI Anda (URL Balasan). Redirect URI, atau URL Balasan, adalah lokasi di mana server otorisasi mengirimkan pengguna setelah aplikasi berhasil diotorisasi dan diberi kode otorisasi atau token Access. Server otorisasi mengirimkan kode atau token ke pengalihan URI; Jadi penting untuk mendaftarkan lokasi yang benar sebagai bagian dari proses pendaftaran aplikasi.

**Penyediaan aplikasi**

[Tutorial: mengembangkan dan merencanakan penyediaan untuk titik akhir scim](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) -artikel ini menguraikan cara menyusun titik akhir scim dan mengintegrasikan dengan layanan penyediaan AAD.


