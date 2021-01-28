---
title: Masalah dengan klaim dan atribut token
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
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035964"
---
# <a name="issues-with-token-claims-and-attributes"></a>Masalah dengan klaim dan atribut token

**Memperbarui, mengonfigurasi, atau menghapus klaim token**

1. Dengan menggunakan Azure Active Directory (Azure AD), Anda dapat [mengustomisasi tipe klaim untuk klaim peran](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) dalam token respons yang Anda terima setelah mengotorisasi aplikasi.
2. Pengembang aplikasi bisa menggunakan klaim opsional dalam aplikasi Azure AD untuk menentukan klaim mana yang mereka inginkan dalam Token yang dikirimkan ke aplikasinya. Untuk informasi selengkapnya, lihat [menyediakan klaim opsional ke aplikasi Anda](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
3. [Mengonfigurasi klaim grup untuk aplikasi dengan Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).
4. Jika menggunakan akses menyeluruh tunggal di aplikasi Anda, lihat [mengkustomisasi klaim yang dikeluarkan dalam TOKEN SAML untuk aplikasi perusahaan](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).

**Pemetaan atribut klaim**

1. Untuk mengonfigurasi kebijakan pemetaan klaim menggunakan PowerShell, lihat [mengkustomisasi klaim yang dipancarkan dalam token untuk aplikasi tertentu dalam penyewa (pratinjau)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
2. Atribut ekstensi skema direktori menyediakan cara untuk menyimpan data tambahan di Azure Active Directory pada objek pengguna dan objek direktori lain seperti grup, detail penyewa, prinsip layanan. Hanya atribut ekstensi pada objek pengguna yang dapat digunakan untuk memancarkan klaim ke aplikasi. [Menggunakan atribut ekstensi skema direktori dalam klaim](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) menjelaskan cara menggunakan atribut ekstensi skema direktori untuk mengirim data pengguna ke aplikasi dalam klaim Token.

Untuk informasi selengkapnya tentang klaim token, lihat:

- [Klaim dalam token Access](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Klaim dalam id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Klaim](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) yang bisa Anda harapkan dalam token id dan token Access yang diterbitkan oleh AZURE AD B2C
- [Referensi klaim token SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
