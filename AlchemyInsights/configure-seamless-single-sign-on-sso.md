---
title: Mengonfigurasi akses menyeluruh (SSO, Single sign-on)
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
- "9384"
ms.openlocfilehash: 32790b23547de36cd2864e85ebae67f54ad91707
ms.sourcegitcommit: 309b9f3e6e2ff622f95bb860d337d2c05b7bbe54
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/15/2021
ms.locfileid: "50841537"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Mengonfigurasi akses menyeluruh (SSO, Single sign-on)

**Mengonfigurasi aplikasi**

1. Anda harus mendapatkan nilai dari vendor aplikasi. Anda dapat memasukkan nilai secara manual atau mengunggah file metadata untuk mengekstrak nilai bidang.
2. Banyak aplikasi telah dikonfigurasikan untuk bekerja dengan Azure AD. Aplikasi ini dicantumkan di Galeri aplikasi yang bisa Anda telusuri saat Anda menambahkan aplikasi ke penyewa Azure AD Anda. [Rangkaian mulai cepat](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) memandu Anda dalam proses.
3. Untuk membuat aplikasi non-Galeri, Anda bisa mengklik **+ buat tombol aplikasi Anda sendiri** dan beri nama untuk aplikasi Anda.
    - Secara default, akan memilih **integrasikan aplikasi lain yang tidak Anda temukan di Galeri** yang merupakan opsi yang tepat untuk aplikasi non-galeri.
    - Setelah Anda menekan **Create** setelah meletakkan nama untuk aplikasinya, itu akan membuat aplikasi non-Galeri Enterprise baru.
    - Lalu, Anda dapat menavigasi **masuk tunggal** di bawah **Kelola** aplikasi tersebut dan Anda akan bisa melihat teknik yang berbeda untuk menerapkannya di lingkungan Anda.

**Mengonfigurasi SSO tanpa batas untuk aplikasi tertentu**

Untuk aplikasi di Galeri, Anda akan menemukan detail, langkah demi langkah, instruksi. Untuk mengakses langkah-langkah, Anda bisa menelusuri daftar tutorial konfigurasi aplikasi di [tutorial konfigurasi aplikasi SaaS](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list).

**Mengonfigurasikan SSO berbasis SAML**

1. [Mulai cepat: menyiapkan single sign-on berbasis SAML (SSO) untuk aplikasi di penyewa Azure Active Directory (AZURE AD) Anda](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso).
2. Untuk mempelajari selengkapnya tentang opsi berbasis SAML untuk akses menyeluruh, lihat [memahami akses menyeluruh berbasis SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on).
3. Untuk mempelajari tentang permintaan dan respons autentikasi 2,0 SAML yang didukung oleh Azure Active Directory (Azure AD) untuk single Sign-On (SSO), lihat [protokol SAML Sign-On tunggal](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol).
4. Untuk mempelajari cara membuat dan mengonfigurasi SAML-based single sign-on (SSO) untuk aplikasi Anda di Azure Active Directory (Azure AD) menggunakan Microsoft graph API, lihat [MENGONFIGURASI SAML-based single sign-on untuk aplikasi Anda menggunakan Microsoft GRAPH api](https://docs.microsoft.com/graph/application-saml-sso-configure-api).
5. Untuk mempelajari cara Azure AD menggunakan protokol SAML, lihat [bagaimana platform identitas Microsoft menggunakan protokol SAML](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference).

**Mengonfigurasi token dan klaim**

1. [Cara: mengustomisasi klaim yang dikeluarkan dalam tanda SAML untuk aplikasi perusahaan](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).
2. Untuk mempelajari cara mengonfigurasi klaim menggunakan PowerShell, lihat [caranya: Mengustomisasi klaim yang dipancarkan dalam token untuk aplikasi tertentu dalam penyewa (pratinjau)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
3. Untuk mempelajari cara mengonfigurasi klaim opsional, lihat [caranya: menyediakan klaim opsional ke aplikasi Anda](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
4. Untuk mempelajari cara menggunakan atribut ekstensi skema direktori untuk mengirim data pengguna ke aplikasi dalam klaim token, lihat [menggunakan atribut ekstensi skema direktori dalam klaim](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions).
5. Untuk mempelajari cara mengonfigurasi masa hidup token, lihat [masa hidup Token yang dapat dikonfigurasikan di platform Microsoft Identity (pratinjau)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
6. [Mengonfigurasi kebijakan seumur hidup Token (pratinjau)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) -dalam artikel ini, kami menelusuri skenario kebijakan umum yang bisa membantu Anda memberlakukan aturan baru untuk seumur hidup. Dalam contoh ini, Anda mempelajari cara membuat kebijakan yang mengharuskan pengguna untuk lebih sering mengautentikasi dalam aplikasi web Anda.

**Memecahkan masalah konfigurasi SSO**

- Untuk tanya jawab umum tentang Azure Active Directory Seamless Single Sign-On (Seamless SSO), lihat [Azure Active Directory Seamless single sign-on: Tanya Jawab Umum](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq).
- Untuk pemecahan masalah informasi tentang masalah umum tentang Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO), lihat [memecahkan masalah masuk tunggal Azure Active Directory mulus](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso).
