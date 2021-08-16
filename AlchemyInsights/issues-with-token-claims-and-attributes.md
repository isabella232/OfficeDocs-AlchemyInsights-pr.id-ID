---
title: Masalah dengan Klaim dan Atribut Token
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
- "9004347"
- "7761"
ms.openlocfilehash: 0c9827ee312d6b236c86f5a2973fa61fdc78c49b8565dd4ceb41f9a3a48140bc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54012887"
---
# <a name="issues-with-token-claims-and-attributes"></a>Masalah dengan Klaim dan Atribut Token

**Memperbarui, mengonfigurasi, atau menghapus klaim token**

1. Dengan menggunakan Azure Active Directory (Azure AD), [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) Anda dapat mengustomisasi tipe klaim untuk klaim peran di token respons yang Anda terima setelah mengotorisasi aplikasi.
2. Pengembang aplikasi dapat menggunakan klaim opsional dalam aplikasi Azure AD mereka untuk menentukan klaim mana yang mereka inginkan di token yang dikirimkan ke aplikasi mereka. Untuk informasi selengkapnya, lihat [Menyediakan klaim opsional untuk aplikasi Anda](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
3. [Mengonfigurasi klaim grup untuk aplikasi dengan Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).
4. Jika menggunakan Akses Masuk Tunggal Tanpa Hambatan di aplikasi Anda, lihat [mengustomisasi klaim](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)yang dikeluarkan di token SAML untuk aplikasi perusahaan.

**Pemetaan Atribut Klaim**

1. Untuk mengonfigurasi kebijakan pemetaan klaim menggunakan PowerShell, lihat Mengustomisasi klaim dalam token untuk [aplikasi tertentu di penyewa (Pratinjau).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
2. Atribut ekstensi skema direktori menyediakan cara untuk menyimpan data tambahan dalam Azure Active Directory objek pengguna dan objek direktori lain seperti grup, detail penyewa, prinsipal layanan. Hanya atribut ekstensi pada objek pengguna yang bisa digunakan untuk e memungkinkan klaim pada aplikasi. [Menggunakan atribut ekstensi skema direktori di klaim](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) menjelaskan cara menggunakan atribut ekstensi skema direktori untuk mengirim data pengguna ke aplikasi di klaim token.

Untuk informasi selengkapnya tentang klaim token, lihat:

- [Klaim dalam token akses](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Klaim di dalam id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Klaim](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) yang dapat Anda harapkan dalam token ID dan token akses yang dikeluarkan oleh Azure AD B2C
- [Referensi klaim token SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
