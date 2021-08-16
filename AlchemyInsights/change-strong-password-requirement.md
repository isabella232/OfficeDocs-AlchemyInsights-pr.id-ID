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
ms.openlocfilehash: 8a82c002bd64a33556b632545e98355e860848d845e122bfea06fbc5ee5dcb90
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070687"
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
