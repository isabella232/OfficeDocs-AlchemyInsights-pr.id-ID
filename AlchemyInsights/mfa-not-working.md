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
ms.openlocfilehash: a415116b9ba437cb13426896119cd1b40d9ab491
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768840"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="9b616-102">Masalah dengan Azure MFA</span><span class="sxs-lookup"><span data-stu-id="9b616-102">Issues with Azure MFA</span></span>
<span data-ttu-id="9b616-103">Ada beberapa hal untuk memeriksa apakah pengguna tidak dapat masuk menggunakan otentikasi multi faktor (MFA)</span><span class="sxs-lookup"><span data-stu-id="9b616-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="9b616-104">Pengguna yang dipakai mungkin diblokir di Azure Active Directory portal.</span><span class="sxs-lookup"><span data-stu-id="9b616-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="9b616-105">Jika itu terjadi, otentikasi upaya untuk pengguna khusus tersebut akan secara otomatis ditolak.</span><span class="sxs-lookup"><span data-stu-id="9b616-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="9b616-106">Silakan ikuti langkah di artikel ini untuk membukanya.</span><span class="sxs-lookup"><span data-stu-id="9b616-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="9b616-107">Jika blokir pengguna tidak membantu atau pengguna tidak diblokir Anda dapat mencoba untuk me-reset MFA untuk pengguna dan mereka akan melalui proses mendaftar lagi.</span><span class="sxs-lookup"><span data-stu-id="9b616-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="9b616-108">Silakan ikuti langkah di artikel ini.</span><span class="sxs-lookup"><span data-stu-id="9b616-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="9b616-109">Jika ini adalah pertama kalinya Anda mengaktifkan MFA dan pengguna tidak dapat login ke klien non-browser seperti Outlook, Skype, dll, mungkin ADAL (Active Directory Authentication Library) tidak diaktifkan pada langganan O365 Anda.</span><span class="sxs-lookup"><span data-stu-id="9b616-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="9b616-110">Dalam hal ini Anda akan perlu untuk terhubung ke Exchange Online PowerShell dan menjalankan cmdlet ini:  *set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*</span><span class="sxs-lookup"><span data-stu-id="9b616-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>