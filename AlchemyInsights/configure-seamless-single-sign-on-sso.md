---
title: Mengonfigurasi Seamless Single Sign-on (SSO)
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
- "9004344"
- "9004357"
- "9384"
- "9863"
ms.openlocfilehash: 62f667cccd0761e081b3f651709fadfec12500e76fd8e30b8649a28e99001e4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53966040"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Mengonfigurasi Seamless Single Sign-on (SSO)

**Mengonfigurasi Aplikasi**

1. Anda akan mendapatkan nilai dari vendor aplikasi. Anda dapat memasukkan nilai atau mengunggah file metadata secara manual untuk mengekstrak nilai bidang.
2. Banyak aplikasi telah dikonfigurasi sebelumnya untuk berfungsi dengan Azure AD. Aplikasi ini tercantum dalam galeri aplikasi yang dapat Anda telusuri ketika menambahkan aplikasi ke penyewa Azure AD. Seri [mulai cepat memandu](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) Anda melalui proses tersebut.
3. Untuk membuat aplikasi non-galeri, Anda bisa mengklik **+ Buat tombol Aplikasi Anda** sendiri dan memberi nama untuk Aplikasi Anda.
    - Secara default, aplikasi akan **memilih Integrasikan aplikasi lain yang** tidak ditemukan dalam galeri yang merupakan opsi yang tepat untuk aplikasi Non-galeri.
    - Setelah Anda **menekan** Buat setelah meletakkan nama untuk aplikasi, Aplikasi Perusahaan Non-galeri akan dibuat.
    - Then, you may navigate to **Single Sign-on under** **Manage** of that application and you will be able to see different techniques for implementing it in your environment.

**Mengonfigurasi SSO Tanpa Hambatan untuk aplikasi tertentu**

Untuk aplikasi dalam galeri, Anda akan menemukan instruksi langkah demi langkah yang mendetail. Untuk mengakses langkah-langkah, Anda dapat menelusuri daftar semua tutorial konfigurasi aplikasi di [tutorial konfigurasi aplikasi SaaS](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list).

**Mengonfigurasi SSO berbasis SAML**

1. Mulai cepat: Menyiapkan akses masuk tunggal (SSO) berbasis SAML untuk aplikasi di penyewa [Azure Active Directory (Azure AD) Anda.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)
2. Untuk mempelajari selengkapnya tentang opsi berbasis SAML untuk akses masuk tunggal, lihat Memahami [akses masuk tunggal berbasis SAML.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on)
3. Untuk mempelajari tentang respons dan permintaan autentikasi SAML 2.0 yang mendukung Azure Active Directory (Azure AD) untuk Akses Sign-On Tunggal (SSO), [lihat Protokol Sign-On SAML Tunggal.](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
4. Untuk mempelajari cara membuat dan mengonfigurasi masuk tunggal (SSO) berbasis SAML untuk aplikasi Anda di Azure Active Directory (Azure AD) menggunakan API Microsoft Graph, lihat Mengonfigurasi akses masuk tunggal berbasis SAML untuk aplikasi Anda menggunakan [API Microsoft Graph.](https://docs.microsoft.com/graph/application-saml-sso-configure-api)
5. Untuk mempelajari cara Azure AD menggunakan protokol SAML, [lihat Bagaimana platform identitas Microsoft menggunakan protokol SAML](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference).

**Konfigurasi Token dan Klaim**

1. [Cara: mengustomisasi klaim yang diterbitkan dalam token SAML untuk aplikasi perusahaan.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)
2. Untuk mempelajari cara mengonfigurasi klaim menggunakan PowerShell, lihat Cara: Kustomisasi klaim yang dibuat di token untuk aplikasi tertentu [di penyewa (Pratinjau).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
3. Untuk mempelajari cara mengonfigurasi klaim opsional, lihat [Cara: Memberikan klaim opsional untuk aplikasi Anda](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
4. Untuk mempelajari cara menggunakan atribut ekstensi skema direktori untuk mengirim data pengguna ke aplikasi di klaim token, lihat Menggunakan atribut ekstensi [skema direktori dalam klaim](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions).
5. Untuk mempelajari cara mengonfigurasi masa berlaku token, lihat [Masa berlaku token yang dapat dikonfigurasi di platform identitas Microsoft (pratinjau).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
6. [Mengonfigurasi kebijakan masa berlaku token (pratinjau)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) - Di artikel ini, kami tinjau skenario kebijakan umum yang dapat membantu Anda memberlakukan aturan baru untuk masa berlaku token. Dalam contoh tersebut, Anda akan mempelajari cara membuat kebijakan yang mengharuskan pengguna untuk lebih sering mengautentikasi di aplikasi web Anda.

**Memecahkan masalah Konfigurasi SSO**

- Untuk tanya jawab umum tentang Azure Active Directory Seamless Single Sign-On (Seamless SSO), [lihat Azure Active Directory Seamless Single Sign-On: Frequently asked questions](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq).
- Untuk informasi pemecahan masalah umum terkait Azure Active Directory Tunggal Tanpa Hambatan (Azure AD) Sign-On (SSO Tanpa Hambatan), lihat Azure Active Directory Akses [Masuk Tunggal Tanpa Hambatan.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso)
