---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: baf3ee808cce1e4da362dd0841c0138d7d9268d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685601"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="52a7d-102">Memblokir autentikasi warisan</span><span class="sxs-lookup"><span data-stu-id="52a7d-102">Blocking legacy authentication</span></span>

<span data-ttu-id="52a7d-103">Autentikasi warisan adalah istilah yang merujuk ke permintaan autentikasi yang dibuat oleh:</span><span class="sxs-lookup"><span data-stu-id="52a7d-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="52a7d-104">Klien Office yang lebih lama yang tidak menggunakan autentikasi modern (misalnya, klien Office 2010).</span><span class="sxs-lookup"><span data-stu-id="52a7d-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="52a7d-105">Klien apa pun yang menggunakan protokol email warisan seperti IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="52a7d-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="52a7d-106">Untuk informasi selengkapnya tentang memblokir autentikasi warisan dan mengaktifkan autentikasi modern, lihat [memblokir autentikasi warisan](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span><span class="sxs-lookup"><span data-stu-id="52a7d-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="52a7d-107">Default keamanan di Azure Active Directory (Azure AD) memudahkan untuk aman dan membantu melindungi organisasi Anda.</span><span class="sxs-lookup"><span data-stu-id="52a7d-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="52a7d-108">Default keamanan berisi pengaturan keamanan yang telah dikonfigurasikan sebelumnya untuk serangan umum.</span><span class="sxs-lookup"><span data-stu-id="52a7d-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="52a7d-109">Untuk informasi selengkapnya tentang keamanan default, lihat [apa itu default keamanan?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="52a7d-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="52a7d-110">**Catatan**: jika penyewa Anda dibuat pada atau setelah 22 oktober, 2019, mungkin Anda mengalami perilaku aman-per-default baru dan telah mengaktifkan default keamanan di penyewa Anda.</span><span class="sxs-lookup"><span data-stu-id="52a7d-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="52a7d-111">Dalam upaya untuk melindungi semua pengguna kami, default keamanan sedang diluncurkan ke semua penyewa baru yang dibuat.</span><span class="sxs-lookup"><span data-stu-id="52a7d-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
