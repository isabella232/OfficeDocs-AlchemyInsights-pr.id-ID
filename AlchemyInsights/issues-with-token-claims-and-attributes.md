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
# <a name="issues-with-token-claims-and-attributes"></a><span data-ttu-id="87ae1-102">Masalah dengan klaim dan atribut token</span><span class="sxs-lookup"><span data-stu-id="87ae1-102">Issues with Token Claims and Attributes</span></span>

<span data-ttu-id="87ae1-103">**Memperbarui, mengonfigurasi, atau menghapus klaim token**</span><span class="sxs-lookup"><span data-stu-id="87ae1-103">**Update, configure or remove token claims**</span></span>

1. <span data-ttu-id="87ae1-104">Dengan menggunakan Azure Active Directory (Azure AD), Anda dapat [mengustomisasi tipe klaim untuk klaim peran](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) dalam token respons yang Anda terima setelah mengotorisasi aplikasi.</span><span class="sxs-lookup"><span data-stu-id="87ae1-104">By using Azure Active Directory (Azure AD), you can [customize the claim type for the role claim](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) in the response token that you receive after you authorize an app.</span></span>
2. <span data-ttu-id="87ae1-105">Pengembang aplikasi bisa menggunakan klaim opsional dalam aplikasi Azure AD untuk menentukan klaim mana yang mereka inginkan dalam Token yang dikirimkan ke aplikasinya.</span><span class="sxs-lookup"><span data-stu-id="87ae1-105">Application developers can use optional claims in their Azure AD applications to specify which claims they want in tokens sent to their application.</span></span> <span data-ttu-id="87ae1-106">Untuk informasi selengkapnya, lihat [menyediakan klaim opsional ke aplikasi Anda](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span><span class="sxs-lookup"><span data-stu-id="87ae1-106">For more information, see [Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span></span>
3. <span data-ttu-id="87ae1-107">[Mengonfigurasi klaim grup untuk aplikasi dengan Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span><span class="sxs-lookup"><span data-stu-id="87ae1-107">[Configure group claims for applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span></span>
4. <span data-ttu-id="87ae1-108">Jika menggunakan akses menyeluruh tunggal di aplikasi Anda, lihat [mengkustomisasi klaim yang dikeluarkan dalam TOKEN SAML untuk aplikasi perusahaan](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span><span class="sxs-lookup"><span data-stu-id="87ae1-108">If using Seamless Single Sign-on in your application, see [customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span></span>

<span data-ttu-id="87ae1-109">**Pemetaan atribut klaim**</span><span class="sxs-lookup"><span data-stu-id="87ae1-109">**Claims Attribute Mapping**</span></span>

1. <span data-ttu-id="87ae1-110">Untuk mengonfigurasi kebijakan pemetaan klaim menggunakan PowerShell, lihat [mengkustomisasi klaim yang dipancarkan dalam token untuk aplikasi tertentu dalam penyewa (pratinjau)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span><span class="sxs-lookup"><span data-stu-id="87ae1-110">To configure claims mapping policy using PowerShell, see [Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span></span>
2. <span data-ttu-id="87ae1-111">Atribut ekstensi skema direktori menyediakan cara untuk menyimpan data tambahan di Azure Active Directory pada objek pengguna dan objek direktori lain seperti grup, detail penyewa, prinsip layanan.</span><span class="sxs-lookup"><span data-stu-id="87ae1-111">Directory schema extension attributes provide a way to store additional data in Azure Active Directory on user objects and other directory objects such as groups, tenant details, service principals.</span></span> <span data-ttu-id="87ae1-112">Hanya atribut ekstensi pada objek pengguna yang dapat digunakan untuk memancarkan klaim ke aplikasi.</span><span class="sxs-lookup"><span data-stu-id="87ae1-112">Only extension attributes on user objects can be used for emitting claims to applications.</span></span> <span data-ttu-id="87ae1-113">[Menggunakan atribut ekstensi skema direktori dalam klaim](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) menjelaskan cara menggunakan atribut ekstensi skema direktori untuk mengirim data pengguna ke aplikasi dalam klaim Token.</span><span class="sxs-lookup"><span data-stu-id="87ae1-113">[Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) describes how to use directory schema extension attributes for sending user data to applications in token claims.</span></span>

<span data-ttu-id="87ae1-114">Untuk informasi selengkapnya tentang klaim token, lihat:</span><span class="sxs-lookup"><span data-stu-id="87ae1-114">For more information on token claims, see:</span></span>

- [<span data-ttu-id="87ae1-115">Klaim dalam token Access</span><span class="sxs-lookup"><span data-stu-id="87ae1-115">Claims in access tokens</span></span>](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [<span data-ttu-id="87ae1-116">Klaim dalam id_token</span><span class="sxs-lookup"><span data-stu-id="87ae1-116">Claims in an id_token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- <span data-ttu-id="87ae1-117">[Klaim](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) yang bisa Anda harapkan dalam token id dan token Access yang diterbitkan oleh AZURE AD B2C</span><span class="sxs-lookup"><span data-stu-id="87ae1-117">[Claims](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) that you can expect in ID tokens and access tokens issued by Azure AD B2C</span></span>
- [<span data-ttu-id="87ae1-118">Referensi klaim token SAML</span><span class="sxs-lookup"><span data-stu-id="87ae1-118">SAML token claims reference</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
