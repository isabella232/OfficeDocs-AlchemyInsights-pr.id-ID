---
title: Masalah dengan MFA
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810487"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="b5bb5-102">Masalah dengan Azure MFA</span><span class="sxs-lookup"><span data-stu-id="b5bb5-102">Issues with Azure MFA</span></span>
<span data-ttu-id="b5bb5-103">Terdapat beberapa hal yang perlu diperiksa jika pengguna tidak dapat masuk menggunakan multi-factor authentication (MFA)</span><span class="sxs-lookup"><span data-stu-id="b5bb5-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="b5bb5-104">Pengguna yang terpengaruh mungkin diblokir dalam Portal Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b5bb5-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="b5bb5-105">Jika demikian, Percobaan autentikasi untuk pengguna tertentu tersebut akan otomatis ditolak.</span><span class="sxs-lookup"><span data-stu-id="b5bb5-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="b5bb5-106">Ikuti langkah-langkah dalam artikel ini untuk membuka blokirnya.</span><span class="sxs-lookup"><span data-stu-id="b5bb5-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="b5bb5-107">Jika membuka blokir pengguna tidak membantu atau pengguna tidak diblokir, Anda dapat mencoba mereset MFA untuk pengguna tersebut dan mereka akan melalui proses pendaftaran lagi.</span><span class="sxs-lookup"><span data-stu-id="b5bb5-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="b5bb5-108">Ikuti langkah-langkah dalam artikel ini.</span><span class="sxs-lookup"><span data-stu-id="b5bb5-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="b5bb5-109">Jika ini adalah kali pertama Anda mengaktifkan MFA dan pengguna tidak dapat masuk ke klien non-browser seperti Outlook, Skype, dll, mungkin ADAL (Pustaka Autentikasi Direktori Aktif) tidak diaktifkan pada langganan O365 Anda.</span><span class="sxs-lookup"><span data-stu-id="b5bb5-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="b5bb5-110">Dalam hal ini, Anda perlu menyambungkan ke Exchange Online Powershell dan menjalankan cmdlet ini:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span><span class="sxs-lookup"><span data-stu-id="b5bb5-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>