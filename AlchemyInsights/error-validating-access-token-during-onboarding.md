---
title: Ada kesalahan validasi kesalahan token Access selama analitik desktop di dalam pesawat
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
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783554"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="cd54f-102">Kesalahan "terjadi kesalahan validasi token Access" selama orientasi analitik desktop</span><span class="sxs-lookup"><span data-stu-id="cd54f-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="cd54f-103">Kesalahan ini biasanya diamati ketika token autentikasi kedaluwarsa.</span><span class="sxs-lookup"><span data-stu-id="cd54f-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="cd54f-104">Biasanya, refresh halaman me-refresh Token.</span><span class="sxs-lookup"><span data-stu-id="cd54f-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="cd54f-105">Namun, masalah ini bisa terjadi jika ada kebijakan akses bersyarat yang diterapkan ke akun yang digunakan untuk analitik desktop di papan.</span><span class="sxs-lookup"><span data-stu-id="cd54f-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="cd54f-106">Anda bisa meninjau log masuk Azure AD di Azure portal untuk melihat apakah ada kegagalan masuk untuk akun yang digunakan untuk orientasi analitik desktop.</span><span class="sxs-lookup"><span data-stu-id="cd54f-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="cd54f-107">Untuk informasi selengkapnya tentang akses bersyarat, kunjungi [merencanakan penggunaan akses bersyarat Anda](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="cd54f-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>