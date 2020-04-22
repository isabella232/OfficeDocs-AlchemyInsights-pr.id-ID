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
# <a name="change-strong-password-requirement"></a>Mengubah persyaratan sandi yang kuat

Microsoft memerlukan sandi yang kuat secara default. 

Dengan menggunakan PowerShell, Anda dapat menonaktifkan sandi yang kuat untuk pengguna tertentu dengan perintah ini:<br>
*Set-MsolUser-UserPrincipalName <UserPrincipalName> -strongpasswordrequired $false*

- [Informasi lebih lanjut tentang kebijakan sandi](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Cara menyambung ke Microsoft 365 dengan PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Informasi lebih lanjut tentang perintah PowerShell MsolUser](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
