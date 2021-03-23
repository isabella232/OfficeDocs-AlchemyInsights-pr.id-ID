---
title: Bekerja dengan pustaka autentikasi
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
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035829"
---
# <a name="working-with-authentication-libraries"></a><span data-ttu-id="19380-102">Bekerja dengan pustaka autentikasi</span><span class="sxs-lookup"><span data-stu-id="19380-102">Working with Authentication Libraries</span></span>

<span data-ttu-id="19380-103">Untuk mengatasi masalah Microsoft Authentication Library (MSAL), lakukan langkah-langkah berikut ini:</span><span class="sxs-lookup"><span data-stu-id="19380-103">To resolve Microsoft Authentication Library (MSAL) issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="19380-104">**Bekerja dengan MSAL**: [pustaka autentikasi platform Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) -artikel ini memperlihatkan dukungan pustaka autentikasi Microsoft untuk beberapa tipe aplikasi.</span><span class="sxs-lookup"><span data-stu-id="19380-104">**Working with MSAL**: [Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) - This article shows Microsoft Authentication Library support for several application types.</span></span> <span data-ttu-id="19380-105">Ini menyertakan link ke kode sumber pustaka; tempat untuk mendapatkan paket untuk proyek aplikasi Anda; dan apakah pustaka mendukung masuk pengguna (autentikasi), akses ke api web yang diproteksi (otorisasi), atau keduanya.</span><span class="sxs-lookup"><span data-stu-id="19380-105">It includes links to library source code; where to get the package for your app's project; and whether the library supports user sign-in (authentication), access to protected web APIs (authorization), or both.</span></span>

2. <span data-ttu-id="19380-106">**Pemecahan masalah autentikasi**: msal mendukung beberapa aliran autentikasi untuk digunakan dalam skenario aplikasi yang berbeda.</span><span class="sxs-lookup"><span data-stu-id="19380-106">**Troubleshoot Authentication**: The MSAL supports several authentication flows for use in different application scenarios.</span></span> <span data-ttu-id="19380-107">Tergantung pada bagaimana aplikasi klien Anda dibangun, MSAL bisa menggunakan satu atau beberapa aliran autentikasi yang didukung oleh platform Microsoft Identity.</span><span class="sxs-lookup"><span data-stu-id="19380-107">Depending on how your client application is built, the MSAL can use one or more of the authentication flows supported by the Microsoft identity platform.</span></span> <span data-ttu-id="19380-108">Aliran ini dapat menghasilkan beberapa tipe token dan kode otorisasi, serta memerlukan token berbeda untuk membuatnya berfungsi.</span><span class="sxs-lookup"><span data-stu-id="19380-108">These flows can produce several types of tokens and authorization codes, and require different tokens to make them work.</span></span>

3. <span data-ttu-id="19380-109">**Token Access**: [token akses platform Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) -Pelajari cara api Anda bisa memvalidasi dan gunakan klaim di dalam token Access.</span><span class="sxs-lookup"><span data-stu-id="19380-109">**Access Tokens**: [Microsoft identity platform access tokens](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - Learn how your API can validate and use the claims inside an access token.</span></span> <span data-ttu-id="19380-110">Semua dokumentasi dalam artikel ini, kecuali yang disebutkan, berlaku hanya untuk Token yang diterbitkan untuk api yang telah Anda daftarkan.</span><span class="sxs-lookup"><span data-stu-id="19380-110">All documentation in this article, except where noted, applies only to tokens issued for APIs you've registered.</span></span> <span data-ttu-id="19380-111">Tidak berlaku untuk Token yang dikeluarkan untuk api milik Microsoft, atau token tersebut tidak dapat digunakan untuk memvalidasi bagaimana platform identitas Microsoft akan menerbitkan token untuk API yang Anda buat.</span><span class="sxs-lookup"><span data-stu-id="19380-111">It does not apply to tokens issued for Microsoft-owned APIs, nor can those tokens be used to validate how the Microsoft identity platform will issue tokens for an API you create.</span></span>

<span data-ttu-id="19380-112">**Akhir dukungan untuk Azure Active Directory Authentication Library (ADAL)**</span><span class="sxs-lookup"><span data-stu-id="19380-112">**End of support for Azure Active Directory Authentication Library (ADAL)**</span></span>

- <span data-ttu-id="19380-113">**Mulai 30 juni 2020,** kami tidak akan lagi menambahkan fitur baru untuk ADAL dan Azure AD graph.</span><span class="sxs-lookup"><span data-stu-id="19380-113">**Starting June 30th, 2020,** we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="19380-114">Kami akan terus menyediakan dukungan teknis dan pembaruan keamanan, namun tidak akan lagi menyediakan pembaruan fitur.</span><span class="sxs-lookup"><span data-stu-id="19380-114">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>
- <span data-ttu-id="19380-115">**Mulai 30 juni 2022,** kami akan mengakhiri dukungan untuk ADAL dan Azure AD graph dan tidak akan lagi menyediakan dukungan teknis atau pembaruan keamanan.</span><span class="sxs-lookup"><span data-stu-id="19380-115">**Starting June 30th, 2022,** we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>
- <span data-ttu-id="19380-116">Aplikasi yang menggunakan ADAL pada versi OS yang sudah ada akan terus berfungsi setelah waktu ini tetapi tidak akan *mendapatkan dukungan teknis atau pembaruan keamanan apa pun*.</span><span class="sxs-lookup"><span data-stu-id="19380-116">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>
- <span data-ttu-id="19380-117">Aplikasi menggunakan grafik Azure AD setelah waktu ini mungkin tidak lagi menerima respons dari titik akhir Azure AD graph.</span><span class="sxs-lookup"><span data-stu-id="19380-117">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="19380-118">**Migrasi ADAL**</span><span class="sxs-lookup"><span data-stu-id="19380-118">**ADAL Migration**</span></span>

- <span data-ttu-id="19380-119">Kami merekomendasikan memperbarui ke MSAL, yang memiliki fitur dan pembaruan keamanan terbaru.</span><span class="sxs-lookup"><span data-stu-id="19380-119">We recommend updating to the MSAL, which has the latest features and security updates.</span></span>
- <span data-ttu-id="19380-120">Jika Anda menggunakan Microsoft Apps, Ketahuilah bahwa Microsoft sedang dalam proses migrasi aplikasinya ke MSAL dengan tenggat waktu dukungan akhir, memastikan mereka akan mendapatkan manfaat dari peningkatan keamanan dan fitur yang sedang berlangsung.</span><span class="sxs-lookup"><span data-stu-id="19380-120">If you're using Microsoft apps, know that Microsoft is in the process of migrating its apps to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="19380-121">[Baca FAQ ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="19380-121">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
2. <span data-ttu-id="19380-122">[Pelajari tentang cara melakukan migrasi aplikasi secara per platform](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).</span><span class="sxs-lookup"><span data-stu-id="19380-122">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).</span></span>
3. <span data-ttu-id="19380-123">Jika, setelah membaca panduan untuk platform aplikasi Anda, Anda memiliki pertanyaan tambahan, Anda bisa memposting di [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) dengan tag [Azure-AD-adal-bantahan] atau membuka masalah dalam repositori GitHub pustaka.</span><span class="sxs-lookup"><span data-stu-id="19380-123">If, after reading the guide for your app's platform, you have additional questions, you can post on [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) with the tag [azure-ad-adal-deprecation] or open an issue in library's GitHub repository.</span></span> <span data-ttu-id="19380-124">Lihat bagian [bahasa dan kerangka](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) dari artikel **ringkasan msal** untuk link ke repo pustaka.</span><span class="sxs-lookup"><span data-stu-id="19380-124">See the [Languages and frameworks](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) section of the **MSAL overview** article for links to each library's repo.</span></span>
4. <span data-ttu-id="19380-125">**Jika Anda memerlukan bantuan memahami aplikasi mana yang menggunakan ADAL**, kami menyarankan agar Anda meninjau semua kode sumber aplikasi Anda.</span><span class="sxs-lookup"><span data-stu-id="19380-125">**If you need help understanding which of your apps use ADAL**, we recommend you review all of your apps' source code.</span></span> <span data-ttu-id="19380-126">Jika ada, hubungi vendor perangkat lunak independen (ISVs) atau penyedia aplikasi.</span><span class="sxs-lookup"><span data-stu-id="19380-126">If applicable, reach out to any Independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="19380-127">Dukungan Microsoft juga dapat menyediakan daftar semua aplikasi non-Microsoft ADAL di penyewa Anda.</span><span class="sxs-lookup"><span data-stu-id="19380-127">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>







