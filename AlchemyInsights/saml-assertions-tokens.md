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
# <a name="saml-assertions-tokens"></a><span data-ttu-id="fd9f8-102">Pernyataan SAML (token)</span><span class="sxs-lookup"><span data-stu-id="fd9f8-102">SAML Assertions (Tokens)</span></span>

1. <span data-ttu-id="fd9f8-103">Token Security Assertions Markup Language (SAML) adalah representasi klaim XML.</span><span class="sxs-lookup"><span data-stu-id="fd9f8-103">Security Assertions Markup Language (SAML) tokens are XML representations of claims.</span></span> <span data-ttu-id="fd9f8-104">Secara default, token SAML Windows Communication Foundation (WCF) digunakan dalam skenario keamanan gabungan adalah Token yang diterbitkan.</span><span class="sxs-lookup"><span data-stu-id="fd9f8-104">By default, SAML tokens Windows Communication Foundation (WCF) uses in federated security scenarios are issued tokens.</span></span> <span data-ttu-id="fd9f8-105">Untuk informasi selengkapnya, lihat [token SAML dan klaim](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span><span class="sxs-lookup"><span data-stu-id="fd9f8-105">For more information, see [SAML Tokens and Claims](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span></span>
2. <span data-ttu-id="fd9f8-106">Platform identitas Microsoft memancarkan beberapa tipe token sekuritas dalam pemrosesan setiap aliran autentikasi.</span><span class="sxs-lookup"><span data-stu-id="fd9f8-106">The Microsoft identity platform emits several types of security tokens in the processing of each authentication flow.</span></span> <span data-ttu-id="fd9f8-107">[Referensi klaim token SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) menjelaskan format, karakteristik keamanan, dan konten token SAML 2,0.</span><span class="sxs-lookup"><span data-stu-id="fd9f8-107">[SAML token claims reference](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) describes the format, security characteristics, and contents of SAML 2.0 tokens.</span></span>
3. <span data-ttu-id="fd9f8-108">Ikuti panduan dalam [masa hidup Token yang dapat dikonfigurasikan di platform Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) untuk memahami cara mengonfigurasi masa hidup Token.</span><span class="sxs-lookup"><span data-stu-id="fd9f8-108">Follow the guidance in [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) to understand how to configure token lifetimes.</span></span>
4. <span data-ttu-id="fd9f8-109">Ikuti langkah-langkah yang diuraikan dalam [artikel ini](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) untuk memahami cara mengonfigurasi enkripsi token SAML Azure AD.</span><span class="sxs-lookup"><span data-stu-id="fd9f8-109">Follow the steps outlined in [this article](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) to understand how to configure Azure AD SAML token encryption.</span></span>
5. <span data-ttu-id="fd9f8-110">Di Azure AD, Anda dapat menyiapkan opsi penandatanganan sertifikat dan algoritme penandatanganan sertifikat.</span><span class="sxs-lookup"><span data-stu-id="fd9f8-110">In Azure AD, you can set up certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="fd9f8-111">Untuk informasi selengkapnya, lihat [opsi penandatanganan sertifikat tingkat lanjut dalam TOKEN SAML untuk aplikasi galeri di Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span><span class="sxs-lookup"><span data-stu-id="fd9f8-111">For more information, see [Advanced certificate signing options in the SAML token for gallery apps in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>
