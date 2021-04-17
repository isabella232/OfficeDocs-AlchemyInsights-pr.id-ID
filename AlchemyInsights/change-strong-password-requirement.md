---
title: Mengubah Persyaratan Kata Sandi yang Kuat
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
- "9000105"
- "1600"
ms.openlocfilehash: cf5cab9a1c2dd4226997d93417dc7104347f8a6e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818471"
---
# <a name="change-strong-password-requirement"></a>Mengubah persyaratan kata sandi yang kuat

Microsoft secara default memerlukan kata sandi yang kuat.

Dengan PowerShell, Anda dapat menonaktifkan kata sandi yang kuat bagi pengguna tertentu dengan perintah ini:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

Untuk menonaktifkan kata sandi yang kuat untuk semua pengguna, gunakan:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [Informasi selengkapnya tentang kebijakan kata sandi](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Cara menyambungkan ke Microsoft 365 dengan PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Informasi selengkapnya tentang perintah MsolUser PowerShell](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
