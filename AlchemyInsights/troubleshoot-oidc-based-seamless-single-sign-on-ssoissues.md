---
title: Memecahkan masalah single sign-on (SSO) berbasis OIDC
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9375"
ms.openlocfilehash: e4ddde6176d9ab021b93e23b3cb363e10b1c1048
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745024"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>Memecahkan masalah single sign-on (SSO) berbasis OIDC

- Untuk mempelajari cara menambahkan aplikasi berbasis OIDC ke penyewa Azure Anda, lihat [mulai cepat: menyiapkan single sign-on (SSO) berbasis oidc untuk aplikasi di penyewa Azure Active Directory (AZURE AD) Anda](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso).
- Untuk detail selengkapnya tentang aplikasi yang menggunakan standar OpenID Connect untuk menerapkan akses terusan, lihat [memahami akses menyeluruh berbasis OIDC](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on).
- Untuk informasi jika Anda memilih untuk menulis kode dengan mengirim dan menangani permintaan HTTP secara langsung atau menggunakan pustaka sumber terbuka pihak ketiga, daripada menggunakan salah satu pustaka open-source kami, lihat [protokol 2,0 dan OpenID Connect di platform Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols).

**Protokol**

1. [Platform identitas Microsoft dan aliran hibah implisit](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) -karakteristik penentu dari hibah implisit adalah bahwa Token (token id atau token Access) dikembalikan langsung dari titik akhir/otorisasi dan bukan titik akhir/Token. Ini sering digunakan sebagai bagian dari aliran kode otorisasi, yang disebut **"aliran hibrid"-mengambil TOKEN ID pada permintaan/otorisasi bersama dengan kode otorisasi**. Artikel ini menguraikan cara memprogram langsung terhadap protokol dalam aplikasi Anda untuk meminta token dari Azure AD.
2. [Platform identitas Microsoft dan alur kode otorisasi oauth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) -otorisasi kode otorisasi OAuth 2,0 dapat digunakan dalam aplikasi yang terinstal di perangkat untuk mendapatkan akses ke sumber daya yang diproteksi, seperti api web. Menggunakan penerapan platform Microsoft Identity 2,0 OAuth, Anda bisa **menambahkan akses masuk dan api ke aplikasi seluler dan desktop Anda**. Artikel ini menguraikan cara memprogram langsung terhadap protokol dalam aplikasi Anda menggunakan bahasa apa pun.
3. [Microsoft Identity platform dan OpenID Connect Protocol](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) -saat Anda menggunakan Microsoft Identity platform implementasi OpenID Connect, Anda bisa menambahkan akses masuk dan api ke aplikasi Anda. Artikel ini memperlihatkan cara melakukan ini secara independen dari bahasa dan menjelaskan cara **mengirim dan menerima pesan http tanpa menggunakan pustaka sumber terbuka Microsoft**.
4. [Platform identitas Microsoft dan alur kredensial klien 2,0 OAuth](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) -Anda bisa menggunakan hibah kredensial klien OAuth 2,0 yang ditentukan dalam RFC 6749, terkadang disebut **OAuth bercabang dua**, untuk mengakses sumber daya yang dihosting web dengan menggunakan identitas aplikasi. Tipe hibah ini biasanya digunakan untuk interaksi server-ke-server yang harus berjalan di latar belakang, tanpa interaksi langsung dengan pengguna. Tipe aplikasi ini sering dirujuk sebagai **daemon** atau **akun Layanan**. Artikel ini menguraikan cara memprogram langsung terhadap protokol dalam aplikasi Anda.
