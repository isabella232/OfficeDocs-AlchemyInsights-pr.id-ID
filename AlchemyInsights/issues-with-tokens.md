---
title: Masalah dengan token
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7774"
- "9004351"
ms.openlocfilehash: 14a9681c08920094813497e7a75eb87bb0733cbc
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917042"
---
# <a name="issues-with-tokens"></a>Masalah dengan token

Untuk mengelola masalah terkait token, Anda bisa melakukan langkah-langkah berikut:

1. Anda dapat menentukan seumur hidup dari Access, ID, atau tanda SAML yang diterbitkan oleh Microsoft Identity platform. Anda dapat mengatur masa pakai token untuk semua aplikasi di organisasi Anda, untuk aplikasi multi-penyewa (multi-organisasi), atau untuk prinsip layanan tertentu di organisasi Anda. Untuk informasi selengkapnya, lihat [masa hidup Token yang dapat dikonfigurasi di platform Microsoft Identity (pratinjau)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
2. Token Access memungkinkan klien untuk menghubungi api web yang dilindungi dengan aman, dan digunakan oleh api web untuk melakukan autentikasi dan otorisasi. Sesuai spesifikasi OAuth, Token Access adalah string yang buram tanpa format yang diatur-beberapa penyedia identitas (IDPs) menggunakan GUID, yang lainnya menggunakan gumpalan terenkripsi. Platform identitas Microsoft menggunakan berbagai format token Access, tergantung pada konfigurasi API yang menerima token. Untuk mempelajari bagaimana API Anda bisa memvalidasi dan menggunakan klaim di dalam token Access, lihat [token akses platform Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/userinfo#calling-the-userinfo-endpoint).
3. Pustaka autentikasi Microsoft (MSAL) mendukung beberapa aliran autentikasi untuk digunakan dalam skenario aplikasi yang berbeda. Untuk informasi selengkapnya, lihat [alur autentikasi](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows#how-each-flow-emits-tokens-and-codes).
4. Pemberian kode otorisasi OAuth 2,0 dapat digunakan dalam aplikasi yang diinstal di perangkat untuk mendapatkan akses ke sumber daya yang diproteksi, seperti api web. Menggunakan penerapan platform Microsoft Identity 2,0 OAuth, Anda bisa menambahkan akses masuk dan API ke aplikasi seluler dan desktop Anda. Lihat [platform Microsoft Identity dan alur kode otorisasi OAuth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token) untuk cara memprogram langsung terhadap protokol dalam aplikasi Anda, menggunakan bahasa apa pun.
5. OpenID Connect (OIDC) adalah protokol autentikasi yang dibangun pada 2,0 OAuth yang bisa Anda gunakan untuk memasukkan pengguna dengan aman ke aplikasi. Saat Anda menggunakan implementasi Microsoft Identity platform Endpoint dari OpenID Connect, Anda bisa menambahkan akses masuk dan API ke aplikasi Anda. [Microsoft Identity platform dan OpenID Connect Protocol](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc#send-the-sign-in-request) memperlihatkan cara melakukan hal ini secara independen dari bahasa dan menjelaskan cara mengirim dan menerima pesan http tanpa menggunakan pustaka sumber terbuka Microsoft.
    - Titik akhir UserInfo adalah bagian dari standar OIDC, didesain untuk mengembalikan klaim tentang pengguna yang diautentikasi. Untuk informasi selengkapnya, lihat [titik akhir UserInfo Microsoft Identity platform](https://docs.microsoft.com/azure/active-directory/develop/userinfo#consider-use-an-id-token-instead).
    - [Panggilan api web dalam aplikasi web menggunakan AZURE AD dan OpenID Connect](https://docs.microsoft.com/samples/azure-samples/active-directory-dotnet-webapp-webapi-openidconnect/active-directory-dotnet-webapp-webapi-openidconnect/) sampel memperlihatkan cara membuat aplikasi web MVC yang menggunakan Azure AD untuk masuk menggunakan protokol Sambungkan OpenID, lalu MEMANGGIL web api di bawah identitas pengguna yang masuk menggunakan token yang diperoleh melalui OAuth 2,0. Sampel ini menggunakan OpenID Connect ASP .net OWIN middleware dan ADAL .net.
6. [Mengonfigurasi aplikasi untuk MENGEKSPOS api web](https://docs.microsoft.com/azure/active-directory/develop/quickstart-configure-app-expose-web-apis) -dalam mulai cepat ini, Anda mendaftarkan api web dengan platform identitas Microsoft dan mengekspos ke aplikasi klien dengan menambahkan contoh lingkup. Dengan mendaftarkan API web dan mengekspos melalui lingkup, Anda dapat memberikan akses berbasis izin ke sumber dayanya kepada pengguna yang sah dan aplikasi klien yang mengakses API Anda.
7. Di Azure Active Directory B2C (Azure AD B2C), aliran kredensial kata sandi sumber daya (ROPC) adalah aliran autentikasi standar OAuth. Dalam alur ini, aplikasi, yang juga dikenal sebagai pihak pengandal, bertukar kredensial yang valid untuk Token. Kredensial menyertakan ID pengguna dan kata sandi. Token yang dikembalikan adalah token ID, Token akses, dan token refresh. Untuk informasi selengkapnya, lihat [menyiapkan aliran kredensial kata sandi pemilik sumber daya di Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/add-ropc-policy?tabs=app-reg-ga&pivots=b2c-user-flow). 

