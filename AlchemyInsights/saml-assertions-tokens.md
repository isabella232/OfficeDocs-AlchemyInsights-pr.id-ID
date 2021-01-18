---
title: Pernyataan SAML (token)
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
- "9004341"
- "7753"
ms.openlocfilehash: 557e23da09df3ab066c2ad7c0352f5fd904b5490
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885217"
---
# <a name="saml-assertions-tokens"></a>Pernyataan SAML (token)

1. Token Security Assertions Markup Language (SAML) adalah representasi klaim XML. Secara default, token SAML Windows Communication Foundation (WCF) digunakan dalam skenario keamanan gabungan adalah Token yang diterbitkan. Untuk informasi selengkapnya, lihat [token SAML dan klaim](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).
2. Platform identitas Microsoft memancarkan beberapa tipe token sekuritas dalam pemrosesan setiap aliran autentikasi. [Referensi klaim token SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) menjelaskan format, karakteristik keamanan, dan konten token SAML 2,0.
3. Ikuti panduan dalam [masa hidup Token yang dapat dikonfigurasikan di platform Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) untuk memahami cara mengonfigurasi masa hidup Token.
4. Ikuti langkah-langkah yang diuraikan dalam [artikel ini](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) untuk memahami cara mengonfigurasi enkripsi token SAML Azure AD.
5. Di Azure AD, Anda dapat menyiapkan opsi penandatanganan sertifikat dan algoritme penandatanganan sertifikat. Untuk informasi selengkapnya, lihat [opsi penandatanganan sertifikat tingkat lanjut dalam TOKEN SAML untuk aplikasi galeri di Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).
