---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: e7bff5f9fcf6f2f2c77e93c2f27f585f2cc18bea
ms.sourcegitcommit: 98231a228ecb2bf14ec3b96d4dd4ccf2507617a3
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/01/2020
ms.locfileid: "43079263"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="f5fa8-102">Memblokir otentikasi lama</span><span class="sxs-lookup"><span data-stu-id="f5fa8-102">Blocking legacy authentication</span></span>

<span data-ttu-id="f5fa8-103">Otentikasi Legacy adalah istilah yang merujuk ke permintaan otentikasi yang dibuat oleh:</span><span class="sxs-lookup"><span data-stu-id="f5fa8-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="f5fa8-104">Klien Office yang lebih lawas yang tidak menggunakan otentikasi modern (misalnya, Office 2010 klien).</span><span class="sxs-lookup"><span data-stu-id="f5fa8-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="f5fa8-105">Setiap klien yang menggunakan protokol mail Legacy seperti IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="f5fa8-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="f5fa8-106">Untuk informasi lebih lanjut tentang memblokir otentikasi Legacy dan mengaktifkan otentikasi modern, lihat [memblokir otentikasi Legacy](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span><span class="sxs-lookup"><span data-stu-id="f5fa8-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="f5fa8-107">Keamanan default di Azure Active Directory (Azure AD) membuatnya lebih mudah untuk menjadi aman dan membantu melindungi organisasi Anda.</span><span class="sxs-lookup"><span data-stu-id="f5fa8-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="f5fa8-108">Keamanan default berisi konfigurasi keamanan yang telah dikonfigurasikan untuk serangan umum.</span><span class="sxs-lookup"><span data-stu-id="f5fa8-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="f5fa8-109">Untuk informasi lebih lanjut tentang default keamanan, lihat [apa itu default keamanan?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="f5fa8-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="f5fa8-110">**Catatan**: jika penyewa Anda dibuat pada atau setelah Oktober 22nd, 2019, itu mungkin Anda mengalami perilaku aman-oleh-default baru dan sudah memiliki default keamanan diaktifkan di penyewa Anda.</span><span class="sxs-lookup"><span data-stu-id="f5fa8-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="f5fa8-111">Dalam upaya untuk melindungi semua pengguna kami, default keamanan sedang digulirkan ke semua penyewa baru dibuat.</span><span class="sxs-lookup"><span data-stu-id="f5fa8-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
