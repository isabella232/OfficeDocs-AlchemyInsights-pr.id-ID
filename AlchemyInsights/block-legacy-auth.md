---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: 06ded694893c020f862864215700853b19d35f08
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820181"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="3a169-102">Memblokir autentikasi warisan</span><span class="sxs-lookup"><span data-stu-id="3a169-102">Blocking legacy authentication</span></span>

<span data-ttu-id="3a169-103">Autentikasi warisan adalah istilah yang merujuk pada permintaan autentikasi yang dibuat oleh:</span><span class="sxs-lookup"><span data-stu-id="3a169-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="3a169-104">Klien Office lama yang tidak menggunakan autentikasi modern (misalnya, klien Office 2010).</span><span class="sxs-lookup"><span data-stu-id="3a169-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="3a169-105">Setiap klien yang menggunakan protokol email warisan seperti IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="3a169-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="3a169-106">Untuk informasi selengkapnya tentang memblokir autentikasi warisan dan mengaktifkan autentikasi modern, lihat [Memblokir autentikasi warisan](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span><span class="sxs-lookup"><span data-stu-id="3a169-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="3a169-107">Keamanan default di Azure Active Directory (Azure AD) memudahkan untuk mengamankan dan membantu melindungi organisasi Anda.</span><span class="sxs-lookup"><span data-stu-id="3a169-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="3a169-108">Default keamanan berisi pengaturan keamanan yang telah dikonfigurasi sebelumnya untuk serangan umum.</span><span class="sxs-lookup"><span data-stu-id="3a169-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="3a169-109">Untuk informasi selengkapnya tentang default keamanan, lihat [Apa itu default keamanan?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="3a169-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="3a169-110">**Catatan**: Jika penyewa dibuat pada atau setelah 22 Oktober 2019, mungkin Anda mengalami perilaku aman secara default yang baru dan telah mengaktifkan default keamanan dalam penyewa.</span><span class="sxs-lookup"><span data-stu-id="3a169-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="3a169-111">Dalam upaya melindungi semua pengguna kami, default keamanan sedang diluncurkan ke semua penyewa baru yang dibuat.</span><span class="sxs-lookup"><span data-stu-id="3a169-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
