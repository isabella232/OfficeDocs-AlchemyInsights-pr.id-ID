---
title: Masalah dengan MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 276f6b2212c9d85df726cb46a46dee7828b34c89
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/25/2019
ms.locfileid: "36545172"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="bd41d-102">Masalah dengan MFA</span><span class="sxs-lookup"><span data-stu-id="bd41d-102">Issues with MFA</span></span>
<span data-ttu-id="bd41d-103">Ada beberapa hal untuk memeriksa apakah pengguna tidak dapat login menggunakan otentikasi multi faktor (MFA)</span><span class="sxs-lookup"><span data-stu-id="bd41d-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="bd41d-104">Pengguna yang dipakai mungkin diblokir di Azure Active Directory portal.</span><span class="sxs-lookup"><span data-stu-id="bd41d-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="bd41d-105">Jika itu terjadi, otentikasi upaya untuk pengguna khusus tersebut akan secara otomatis ditolak.</span><span class="sxs-lookup"><span data-stu-id="bd41d-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="bd41d-106">Silakan ikuti langkah di artikel ini untuk membukanya.</span><span class="sxs-lookup"><span data-stu-id="bd41d-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="bd41d-107">Jika blokir pengguna tidak membantu atau pengguna tidak diblokir Anda dapat mencoba untuk me-reset MFA untuk pengguna dan mereka akan melalui proses mendaftar lagi.</span><span class="sxs-lookup"><span data-stu-id="bd41d-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="bd41d-108">Silakan ikuti langkah di artikel ini.</span><span class="sxs-lookup"><span data-stu-id="bd41d-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="bd41d-109">Jika ini adalah pertama kalinya Anda mengaktifkan MFA dan pengguna tidak dapat login ke klien non-browser seperti Outlook, Skype, dll, mungkin ADAL (Active Directory Authentication Library) tidak diaktifkan pada langganan O365 Anda.</span><span class="sxs-lookup"><span data-stu-id="bd41d-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="bd41d-110">Dalam hal ini Anda akan perlu untuk terhubung ke Exchange Online PowerShell dan menjalankan cmdlet ini:  *set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*</span><span class="sxs-lookup"><span data-stu-id="bd41d-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>