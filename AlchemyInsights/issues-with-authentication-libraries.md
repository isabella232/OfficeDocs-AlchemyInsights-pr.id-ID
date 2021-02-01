---
title: Masalah dengan pustaka autentikasi
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
- "9004333"
- "7731"
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063636"
---
# <a name="issues-with-authentication-libraries"></a><span data-ttu-id="9f63d-102">Masalah dengan pustaka autentikasi</span><span class="sxs-lookup"><span data-stu-id="9f63d-102">Issues with Authentication Libraries</span></span>

1. <span data-ttu-id="9f63d-103">[Pustaka autentikasi platform identitas Microsoft](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) mencantumkan pustaka klien dan middleware yang didukung Microsoft dan kompatibel.</span><span class="sxs-lookup"><span data-stu-id="9f63d-103">[Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) lists Microsoft-supported and compatible client and middleware libraries.</span></span>
2. <span data-ttu-id="9f63d-104">Pustaka autentikasi Microsoft (MSAL) mendukung beberapa [aliran autentikasi](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) untuk digunakan dalam skenario aplikasi yang berbeda.</span><span class="sxs-lookup"><span data-stu-id="9f63d-104">The Microsoft Authentication Library (MSAL) supports several [authentication flows](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) for use in different application scenarios.</span></span>
3. <span data-ttu-id="9f63d-105">Untuk mengautentikasi dan memperoleh token, Anda menginisialisasi aplikasi klien publik atau rahasia baru di kode Anda.</span><span class="sxs-lookup"><span data-stu-id="9f63d-105">To authenticate and acquire tokens, you initialize a new public or confidential client application in your code.</span></span> <span data-ttu-id="9f63d-106">Anda bisa mengatur beberapa opsi konfigurasi saat Anda menginisialisasi aplikasi klien di pustaka autentikasi Microsoft (MSAL).</span><span class="sxs-lookup"><span data-stu-id="9f63d-106">You can set several configuration options when you initialize the client app in the Microsoft Authentication Library (MSAL).</span></span> <span data-ttu-id="9f63d-107">Untuk mempelajari selengkapnya, lihat [opsi konfigurasi aplikasi](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span><span class="sxs-lookup"><span data-stu-id="9f63d-107">To learn more, see [Application configuration options](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span></span>

<span data-ttu-id="9f63d-108">**Akhir dukungan untuk Azure Active Directory Authentication Library (ADAL) dan Azure AD graph API (Graf AAD)**</span><span class="sxs-lookup"><span data-stu-id="9f63d-108">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="9f63d-109">**Mulai 30 juni 2020**, kami tidak akan lagi menambahkan fitur baru untuk ADAL dan Azure AD graph.</span><span class="sxs-lookup"><span data-stu-id="9f63d-109">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="9f63d-110">Kami akan terus menyediakan dukungan teknis dan pembaruan keamanan, namun tidak akan lagi menyediakan pembaruan fitur.</span><span class="sxs-lookup"><span data-stu-id="9f63d-110">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="9f63d-111">**Mulai 30 juni 2022**, kami akan mengakhiri dukungan untuk ADAL dan Azure AD graph dan tidak akan lagi menyediakan dukungan teknis atau pembaruan keamanan.</span><span class="sxs-lookup"><span data-stu-id="9f63d-111">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="9f63d-112">Aplikasi yang menggunakan ADAL pada versi OS yang sudah ada akan terus berfungsi setelah waktu ini tetapi tidak akan *mendapatkan dukungan teknis atau pembaruan keamanan apa pun*.</span><span class="sxs-lookup"><span data-stu-id="9f63d-112">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="9f63d-113">Aplikasi menggunakan grafik Azure AD setelah waktu ini mungkin tidak lagi menerima respons dari titik akhir Azure AD graph.</span><span class="sxs-lookup"><span data-stu-id="9f63d-113">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="9f63d-114">**Migrasi ADAL**</span><span class="sxs-lookup"><span data-stu-id="9f63d-114">**ADAL Migration**</span></span>

<span data-ttu-id="9f63d-115">Kami merekomendasikan Anda memperbarui ke [Pustaka Autentikasi Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), yang memiliki fitur dan pembaruan keamanan terbaru.</span><span class="sxs-lookup"><span data-stu-id="9f63d-115">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="9f63d-116">Jika Anda menggunakan Microsoft Apps, Ketahuilah bahwa Microsoft sedang dalam proses migrasi aplikasinya ke MSAL dengan tenggat waktu dukungan akhir, memastikan mereka akan mendapatkan manfaat dari keamanan dan penyempurnaan fitur yang sedang berlangsung.</span><span class="sxs-lookup"><span data-stu-id="9f63d-116">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they will benefit from MSAL's ongoing security and feature improvements.</span></span>

<span data-ttu-id="9f63d-117">Untuk informasi selengkapnya, lihat:</span><span class="sxs-lookup"><span data-stu-id="9f63d-117">For more information, see:</span></span>

1. [<span data-ttu-id="9f63d-118">Baca FAQ ADAL</span><span class="sxs-lookup"><span data-stu-id="9f63d-118">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="9f63d-119">Pelajari tentang cara melakukan migrasi aplikasi pada basis per platform</span><span class="sxs-lookup"><span data-stu-id="9f63d-119">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="9f63d-120">Jika Anda memerlukan bantuan untuk memahami aplikasi mana yang menggunakan ADAL, kami menyarankan agar Anda meninjau semua kode sumber aplikasi Anda, dan jika ada, hubungi penyedia ISVs atau aplikasi apa pun.</span><span class="sxs-lookup"><span data-stu-id="9f63d-120">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="9f63d-121">Dukungan Microsoft juga dapat menyediakan daftar semua aplikasi non-Microsoft ADAL di penyewa Anda.</span><span class="sxs-lookup"><span data-stu-id="9f63d-121">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="9f63d-122">**Migrasi Grafik AAD**</span><span class="sxs-lookup"><span data-stu-id="9f63d-122">**AAD Graph Migration**</span></span>

<span data-ttu-id="9f63d-123">Untuk aplikasi yang menggunakan Azure AD graph, ikuti panduan kami untuk melakukan [migrasi aplikasi AZURE AD graph ke Microsoft graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span><span class="sxs-lookup"><span data-stu-id="9f63d-123">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. [<span data-ttu-id="9f63d-124">Daftar Periksa migrasi kami menyediakan titik mulai.</span><span class="sxs-lookup"><span data-stu-id="9f63d-124">Our migration checklist provides a getting started point.</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. <span data-ttu-id="9f63d-125">Portal pendaftaran aplikasi Azure Anda memperlihatkan aplikasi mana yang menggunakan Grafik AAD.</span><span class="sxs-lookup"><span data-stu-id="9f63d-125">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="9f63d-126">Kami menyarankan Anda meninjau semua kode sumber aplikasi, dan jika memungkinkan, hubungi semua ISV atau penyedia aplikasi.</span><span class="sxs-lookup"><span data-stu-id="9f63d-126">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="9f63d-127">Dukungan Microsoft juga bisa memberi Anda daftar semua penggunaan grafik AAD dalam penyewa Anda.</span><span class="sxs-lookup"><span data-stu-id="9f63d-127">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="9f63d-128">Agar aplikasi Anda dapat mengakses data di Microsoft graph, pengguna atau administrator harus memberinya izin yang benar melalui proses persetujuan.</span><span class="sxs-lookup"><span data-stu-id="9f63d-128">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="9f63d-129">[Referensi izin Microsoft graph](https://docs.microsoft.com/graph/permissions-reference) mencantumkan izin yang terkait dengan setiap kumpulan utama api Microsoft graph.</span><span class="sxs-lookup"><span data-stu-id="9f63d-129">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="9f63d-130">Ini juga memberikan panduan tentang cara menggunakan izin.</span><span class="sxs-lookup"><span data-stu-id="9f63d-130">It also provides guidance about how to use the permissions.</span></span>
