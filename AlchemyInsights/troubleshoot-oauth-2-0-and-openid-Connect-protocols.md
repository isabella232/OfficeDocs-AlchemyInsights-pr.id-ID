---
title: Memecahkan masalah protokol OAuth 2,0 dan OpenID Connect
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9776"
- "9004342"
ms.openlocfilehash: d2f14d4d16bea890b564cdb9bd9ac3875c28d115
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036405"
---
# <a name="troubleshoot-oauth-20-and-openid-connect-protocols"></a><span data-ttu-id="d43d3-102">Memecahkan masalah protokol OAuth 2,0 dan OpenID Connect</span><span class="sxs-lookup"><span data-stu-id="d43d3-102">Troubleshoot OAuth 2.0 and OpenID Connect protocols</span></span>

<span data-ttu-id="d43d3-103">Untuk mengatasi masalah OAuth 2,0 dan OpenID Connect, lakukan langkah-langkah berikut ini:</span><span class="sxs-lookup"><span data-stu-id="d43d3-103">To resolve OAuth 2.0 and OpenID Connect issues, perform the following recommended steps:</span></span>

<span data-ttu-id="d43d3-104">Lihat artikel berikut yang terkait dengan konfigurasi dan pemecahan masalah protokol koneksi OAuth 2,0 dan OpenID:</span><span class="sxs-lookup"><span data-stu-id="d43d3-104">Refer to the following articles that are related to configuration and troubleshooting OAuth 2.0 and OpenID Connect protocols:</span></span>

- <span data-ttu-id="d43d3-105">[Alur kode Microsoft Identity platform dan OAuth 2,0 otorisasi](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) -artikel ini menjelaskan cara memprogram langsung terhadap **aliran Code Grant (pkce)** dalam aplikasi Anda, menggunakan bahasa apa pun.</span><span class="sxs-lookup"><span data-stu-id="d43d3-105">[Microsoft identity platform and OAuth 2.0 authorization code flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) - This article describes how to program directly against the **code grant (PKCE) flow** in your application, using any language.</span></span>
- <span data-ttu-id="d43d3-106">[Platform identitas Microsoft dan alur kredensial klien 2,0 OAuth](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) -artikel ini menguraikan cara program langsung terhadap **aliran kredensial klien** dalam aplikasi Anda.</span><span class="sxs-lookup"><span data-stu-id="d43d3-106">[Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) - This article describes how to program directly against the **client credentials flow** in your application.</span></span>
- <span data-ttu-id="d43d3-107">[Kredensial kata sandi Microsoft Identity platform dan sumber daya 2,0 OAuth](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth-ropc) -artikel ini menjelaskan cara memprogram langsung terhadap **aliran ropc** dalam aplikasi Anda.</span><span class="sxs-lookup"><span data-stu-id="d43d3-107">[Microsoft identity platform and OAuth 2.0 Resource Owner Password Credentials](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth-ropc) - This article describes how to program directly against the **ROPC flow** in your application.</span></span>
    - <span data-ttu-id="d43d3-108">Platform identitas Microsoft hanya mendukung ROPC untuk penyewa Azure AD, dan bukan untuk akun pribadi.</span><span class="sxs-lookup"><span data-stu-id="d43d3-108">The Microsoft identity platform only supports ROPC for Azure AD tenants, and not for personal accounts.</span></span> <span data-ttu-id="d43d3-109">Ini berarti bahwa Anda harus menggunakan titik akhir penyewa-spesifik **( https://login.microsoftonline.com/{TenantId_or_Name})** atau titik akhir **organisasi** .</span><span class="sxs-lookup"><span data-stu-id="d43d3-109">This means that you must use a tenant-specific endpoint **(https://login.microsoftonline.com/{TenantId_or_Name})** or the **organizations** endpoint.</span></span>
    - <span data-ttu-id="d43d3-110">Akun pribadi yang diundang ke penyewa Azure AD tidak dapat menggunakan ROPC.</span><span class="sxs-lookup"><span data-stu-id="d43d3-110">Personal accounts that are invited to an Azure AD tenant can't use ROPC.</span></span>
    - <span data-ttu-id="d43d3-111">Akun yang tidak memiliki kata sandi tidak bisa masuk melalui ROPC.</span><span class="sxs-lookup"><span data-stu-id="d43d3-111">Accounts that don't have passwords can't sign in through ROPC.</span></span> <span data-ttu-id="d43d3-112">Untuk skenario ini, kami menyarankan agar Anda menggunakan aliran berbeda untuk aplikasi Anda.</span><span class="sxs-lookup"><span data-stu-id="d43d3-112">For this scenario, we recommend that you use a different flow for your app, instead.</span></span>
    - <span data-ttu-id="d43d3-113">Jika pengguna perlu menggunakan [multi-Factor Authentication (MFA)](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-howitworks) untuk masuk ke aplikasi, maka mereka akan diblokir.</span><span class="sxs-lookup"><span data-stu-id="d43d3-113">If users need to use [multi-factor authentication (MFA)](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-howitworks) to log in to the application, they will be blocked.</span></span>
    - <span data-ttu-id="d43d3-114">ROPC tidak didukung dalam skenario [Federasi identitas hibrid](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-fed) (misalnya, Azure AD dan ADFS yang digunakan untuk mengotentikasi akun lokal).</span><span class="sxs-lookup"><span data-stu-id="d43d3-114">ROPC is not supported in [hybrid identity federation](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-fed) scenarios (for example, Azure AD and ADFS used to authenticate on-premises accounts).</span></span> <span data-ttu-id="d43d3-115">Jika pengguna memiliki halaman penuh dialihkan ke penyedia identitas lokal, Azure AD tidak dapat menguji nama pengguna dan kata sandi terhadap penyedia identitas tersebut.</span><span class="sxs-lookup"><span data-stu-id="d43d3-115">If users are full-page redirected to an on-premises identity provider, Azure AD is not able to test the username and password against that identity provider.</span></span> <span data-ttu-id="d43d3-116">[Autentikasi kirim](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta) langsung didukung dengan ropc.</span><span class="sxs-lookup"><span data-stu-id="d43d3-116">[Pass-through authentication](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta) is supported with ROPC, however.</span></span>
    - <span data-ttu-id="d43d3-117">Pengecualian untuk skenario Federasi identitas hibrid adalah sebagai berikut: kebijakan penemuan Realm rumah dengan kumpulan **pengesahan Allowcloudpassworddiatur** ke **True** akan mengaktifkan aliran ropc agar berfungsi bagi pengguna yang tergabung saat kata sandi lokal disinkronkan ke awan.</span><span class="sxs-lookup"><span data-stu-id="d43d3-117">An exception to a hybrid identity federation scenario would be the following: Home Realm Discovery policy with **AllowCloudPasswordValidation** set to **TRUE** will enable ROPC flow to work for federated users when on-premises password is synced to cloud.</span></span> <span data-ttu-id="d43d3-118">Untuk informasi selengkapnya, lihat [mengaktifkan autentikasi langsung pengguna gabungan untuk aplikasi warisan](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#enable-direct-ropc-authentication-of-federated-users-for-legacy-applications)</span><span class="sxs-lookup"><span data-stu-id="d43d3-118">For more information, see [Enable direct ROPC authentication of federated users for legacy applications](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#enable-direct-ropc-authentication-of-federated-users-for-legacy-applications)</span></span> 
- <span data-ttu-id="d43d3-119">[Platform identitas Microsoft dan 2,0 OAuth atas nama-aliran](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) -artikel ini menjelaskan cara memprogram secara langsung terhadap **aliran di atas nama (OBO)** dalam aplikasi Anda.</span><span class="sxs-lookup"><span data-stu-id="d43d3-119">[Microsoft identity platform and OAuth 2.0 On-Behalf-Of flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) - This article describes how to program directly against the **on-behalf-of (OBO) flow** in your application.</span></span>
- <span data-ttu-id="d43d3-120">[Microsoft Identity platform dan OpenID Connect Protocol](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) -artikel ini memperlihatkan cara menerapkan protokol OpenID Connect independen dari bahasa, dan menjelaskan cara untuk mengirim dan menerima pesan http tanpa menggunakan pustaka sumber terbuka Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d43d3-120">[Microsoft identity platform and OpenID Connect protocol](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) - This article shows how to implement the OpenID Connect protocol independent of language, and describes how to send and receive HTTP messages without using any Microsoft open-source libraries.</span></span>

<span data-ttu-id="d43d3-121">**Token Access**</span><span class="sxs-lookup"><span data-stu-id="d43d3-121">**Access Tokens**</span></span>

<span data-ttu-id="d43d3-122">[Token Access platform identitas Microsoft](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) -Pelajari bagaimana api Anda bisa memvalidasi dan menggunakan klaim di dalam token Access.</span><span class="sxs-lookup"><span data-stu-id="d43d3-122">[Microsoft identity platform access tokens](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - Learn how your API can validate and use the claims inside an access token.</span></span> <span data-ttu-id="d43d3-123">Semua dokumentasi dalam artikel ini, kecuali yang disebutkan, berlaku hanya untuk Token yang diterbitkan untuk api yang telah Anda daftarkan.</span><span class="sxs-lookup"><span data-stu-id="d43d3-123">All documentation in this article, except where noted, applies only to tokens issued for APIs you've registered.</span></span> <span data-ttu-id="d43d3-124">Tidak berlaku untuk Token yang dikeluarkan untuk api milik Microsoft, atau token tersebut tidak dapat digunakan untuk memvalidasi bagaimana platform identitas Microsoft akan menerbitkan token untuk API yang Anda buat.</span><span class="sxs-lookup"><span data-stu-id="d43d3-124">It does not apply to tokens issued for Microsoft-owned APIs, nor can those tokens be used to validate how the Microsoft identity platform will issue tokens for an API you create.</span></span>

<span data-ttu-id="d43d3-125">**Konfigurasi aplikasi**</span><span class="sxs-lookup"><span data-stu-id="d43d3-125">**Application Configuration**</span></span>

<span data-ttu-id="d43d3-126">[Pembatasan dan pembatasan URI redirect (URL Balasan)](https://docs.microsoft.com/azure/active-directory/develop/reply-url) -Pelajari cara MENGONFIGURASI pengalihan URI Anda (URL Balasan).</span><span class="sxs-lookup"><span data-stu-id="d43d3-126">[Redirect URI (reply URL) restrictions and limitations](https://docs.microsoft.com/azure/active-directory/develop/reply-url) - Learn how to configure your Redirect URI (reply URL).</span></span> <span data-ttu-id="d43d3-127">Redirect URI, atau URL Balasan, adalah lokasi di mana server otorisasi mengirimkan pengguna setelah aplikasi berhasil diotorisasi dan diberi kode otorisasi atau token Access.</span><span class="sxs-lookup"><span data-stu-id="d43d3-127">A redirect URI, or reply URL, is the location where the authorization server sends the user once the app has been successfully authorized and granted an authorization code or access token.</span></span> <span data-ttu-id="d43d3-128">Server otorisasi mengirimkan kode atau token ke pengalihan URI; Jadi penting untuk mendaftarkan lokasi yang benar sebagai bagian dari proses pendaftaran aplikasi.</span><span class="sxs-lookup"><span data-stu-id="d43d3-128">The authorization server sends the code or token to the redirect URI; so it's important you register the correct location as part of the app registration process.</span></span>

<span data-ttu-id="d43d3-129">**Penyediaan aplikasi**</span><span class="sxs-lookup"><span data-stu-id="d43d3-129">**Application Provisioning**</span></span>

<span data-ttu-id="d43d3-130">[Tutorial: mengembangkan dan merencanakan penyediaan untuk titik akhir scim](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) -artikel ini menguraikan cara menyusun titik akhir scim dan mengintegrasikan dengan layanan penyediaan AAD.</span><span class="sxs-lookup"><span data-stu-id="d43d3-130">[Tutorial: Develop and plan provisioning for a SCIM endpoint](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) - This article describes how to build an SCIM endpoint and integrate with the AAD provisioning service.</span></span>

