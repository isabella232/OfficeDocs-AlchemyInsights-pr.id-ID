---
title: Ada kesalahan memvalidasi galat token akses selama desktop Analytics on-boarding
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741202"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="ef2ee-102">Galat "ada kesalahan memvalidasi akses token" selama desktop Analytics onboarding</span><span class="sxs-lookup"><span data-stu-id="ef2ee-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="ef2ee-103">Galat ini biasanya diamati saat token otentikasi kedaluwarsa.</span><span class="sxs-lookup"><span data-stu-id="ef2ee-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="ef2ee-104">Biasanya, menyegarkan halaman menyegarkan Token.</span><span class="sxs-lookup"><span data-stu-id="ef2ee-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="ef2ee-105">Namun, masalah ini dapat bertahan jika ada kebijakan akses bersyarat yang diterapkan ke akun yang digunakan untuk di papan desktop Analytics.</span><span class="sxs-lookup"><span data-stu-id="ef2ee-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="ef2ee-106">Anda dapat meninjau Azure AD masuk log di Azure portal untuk melihat apakah ada kegagalan masuk untuk akun yang digunakan untuk onboarding desktop Analytics.</span><span class="sxs-lookup"><span data-stu-id="ef2ee-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="ef2ee-107">Untuk informasi lebih lanjut tentang akses bersyarat, kunjungi [rencanakan penyebaran akses bersyarat Anda](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="ef2ee-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>