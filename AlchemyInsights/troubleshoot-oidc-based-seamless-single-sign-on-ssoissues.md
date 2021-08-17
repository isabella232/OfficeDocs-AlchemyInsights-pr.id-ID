---
title: Memecahkan masalah Masuk Tunggal Tanpa Hambatan (SSO, Seamless Single Sign-on) berbasis OID
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
ms.openlocfilehash: 5880ee37a2fcc98b34231cc9960fb3f87fa184b07bd81ccd37d0ea5a78170af0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105781"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>Memecahkan masalah Masuk Tunggal Tanpa Hambatan (SSO, Seamless Single Sign-on) berbasis OID

- Untuk mempelajari cara menambahkan aplikasi berbasis OIDC ke penyewa Azure Anda, lihat Mulai cepat: Menyiapkan masuk tunggal [(SSO) berbasis OIDC](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso)untuk aplikasi di penyewa Azure Active Directory (Azure AD) Anda.
- Untuk detail selengkapnya tentang aplikasi yang menggunakan openID Koneksi standar untuk menerapkan akses masuk tunggal, lihat Memahami akses masuk tunggal [berbasis OIDC.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on)
- Untuk informasi jika Anda memilih untuk menulis kode dengan mengirim dan menangani permintaan HTTP secara langsung atau menggunakan pustaka sumber terbuka pihak ketiga daripada menggunakan salah satu pustaka sumber terbuka kami, lihat [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols)dan Protokol Koneksi OpenID di platform identitas Microsoft .

**Protokol**

1. platform identitas Microsoft dan aliran pemberian [implisit](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) - Karakteristik pasti pemberian implisit adalah token (token ID atau token akses) dikembalikan secara langsung dari titik akhir /authorize, bukan titik akhir /token. Ini sering digunakan sebagai bagian dari aliran kode otorisasi, di dalam apa yang disebut **"aliran hibrid" -** mengambil token ID di /permintaan otorisasi bersama dengan kode otorisasi . Artikel ini menjelaskan cara memprogram secara langsung terhadap protokol dalam aplikasi Anda untuk meminta token dari Azure AD.
2. platform identitas Microsoft dan aliran kode otorisasi [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) - Pemberian kode otorisasi OAuth 2.0 dapat digunakan di aplikasi yang diinstal di perangkat untuk mendapatkan akses ke sumber daya yang diproteksi, seperti WEB API. Dengan platform identitas Microsoft OAuth 2.0, Anda dapat menambahkan akses masuk dan API ke **aplikasi seluler dan desktop.** Artikel ini menjelaskan cara memprogram protokol secara langsung terhadap protokol dalam aplikasi Anda menggunakan bahasa apa pun.
3. platform identitas Microsoft dan [protokol Koneksi OpenID](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) - Ketika menggunakan penerapan platform identitas Microsoft openID Koneksi, Anda dapat menambahkan akses masuk dan API ke aplikasi. Artikel ini memperlihatkan cara melakukan ini bebas dari bahasa dan menjelaskan cara mengirim dan menerima pesan HTTP tanpa menggunakan pustaka sumber terbuka Microsoft apa **pun.**
4. platform identitas Microsoft dan aliran kredensial klien [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) - Anda dapat menggunakan pemberian kredensial klien OAuth 2.0 yang ditentukan dalam RFC 6749, terkadang disebut **OAuth** dua kaki untuk mengakses sumber daya yang dihosting web menggunakan identitas aplikasi. Jenis pemberian ini umumnya digunakan untuk interaksi server-ke-server yang harus berjalan di latar belakang, tanpa interaksi langsung dengan pengguna. Tipe aplikasi ini sering disebut sebagai **daemon atau akun** **layanan.** Artikel ini menjelaskan cara memprogram secara langsung terhadap protokol dalam aplikasi Anda.
