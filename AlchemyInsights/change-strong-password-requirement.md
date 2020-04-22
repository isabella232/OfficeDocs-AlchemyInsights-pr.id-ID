---
title: Ubah persyaratan sandi yang kuat
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: a054735a0c139c90d76098297bb9984d37464d3b
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706564"
---
# <a name="change-strong-password-requirement"></a><span data-ttu-id="47f78-102">Mengubah persyaratan sandi yang kuat</span><span class="sxs-lookup"><span data-stu-id="47f78-102">Change strong password requirement</span></span>

<span data-ttu-id="47f78-103">Microsoft memerlukan sandi yang kuat secara default.</span><span class="sxs-lookup"><span data-stu-id="47f78-103">Microsoft requires strong passwords by default.</span></span> 

<span data-ttu-id="47f78-104">Dengan menggunakan PowerShell, Anda dapat menonaktifkan sandi yang kuat untuk pengguna tertentu dengan perintah ini:</span><span class="sxs-lookup"><span data-stu-id="47f78-104">Using PowerShell, you can disable strong passwords for specific users with this command:</span></span><br>
<span data-ttu-id="47f78-105">*Set-MsolUser-UserPrincipalName <UserPrincipalName> -strongpasswordrequired $false*</span><span class="sxs-lookup"><span data-stu-id="47f78-105">*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false*</span></span>

- [<span data-ttu-id="47f78-106">Informasi lebih lanjut tentang kebijakan sandi</span><span class="sxs-lookup"><span data-stu-id="47f78-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="47f78-107">Cara menyambung ke Microsoft 365 dengan PowerShell</span><span class="sxs-lookup"><span data-stu-id="47f78-107">How to connect to Microsoft 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="47f78-108">Informasi lebih lanjut tentang perintah PowerShell MsolUser</span><span class="sxs-lookup"><span data-stu-id="47f78-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
