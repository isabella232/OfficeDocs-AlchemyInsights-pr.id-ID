---
title: Masalah dengan MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755134"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="65375-102">Masalah dengan Azure MFA</span><span class="sxs-lookup"><span data-stu-id="65375-102">Issues with Azure MFA</span></span>
<span data-ttu-id="65375-103">Ada beberapa hal untuk diperiksa jika pengguna tidak bisa masuk menggunakan multi-Factor Authentication (MFA)</span><span class="sxs-lookup"><span data-stu-id="65375-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="65375-104">Pengguna yang terpengaruh mungkin diblokir di portal Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="65375-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="65375-105">Jika demikian, upaya autentikasi untuk pengguna tertentu tersebut akan secara otomatis ditolak.</span><span class="sxs-lookup"><span data-stu-id="65375-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="65375-106">Ikuti langkah-langkah dalam artikel ini untuk membuka blokir.</span><span class="sxs-lookup"><span data-stu-id="65375-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="65375-107">Jika membuka blokir pengguna tidak membantu atau pengguna tidak diblokir, Anda bisa mencoba mengatur ulang MFA untuk pengguna dan mereka akan melewati proses pendaftaran lagi.</span><span class="sxs-lookup"><span data-stu-id="65375-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="65375-108">Ikuti langkah-langkah di artikel ini.</span><span class="sxs-lookup"><span data-stu-id="65375-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="65375-109">Jika ini pertama kalinya Anda mengaktifkan MFA dan pengguna Anda tidak dapat masuk ke klien non-browser seperti Outlook, Skype, dll, mungkin ADAL (pustaka autentikasi direktori aktif) tidak diaktifkan pada langganan O365 Anda.</span><span class="sxs-lookup"><span data-stu-id="65375-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="65375-110">Dalam kasus ini, Anda perlu menyambungkan ke Exchange Online PowerShell dan menjalankan cmdlet ini:  *set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*</span><span class="sxs-lookup"><span data-stu-id="65375-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>