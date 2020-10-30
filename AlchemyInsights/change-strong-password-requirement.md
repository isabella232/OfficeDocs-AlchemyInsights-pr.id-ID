---
title: Mengubah persyaratan kata sandi yang kuat
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
- "9000105"
- "1600"
ms.openlocfilehash: 8ce331275e066b5a4f177ae27178ec726f90762f
ms.sourcegitcommit: aa35d2e1829f7d07f64fb891bf73b1fd80f0864c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/30/2020
ms.locfileid: "48804426"
---
# <a name="change-strong-password-requirement"></a>Mengubah persyaratan kata sandi yang kuat

Microsoft memerlukan kata sandi yang kuat secara default.

Menggunakan PowerShell, Anda bisa menonaktifkan kata sandi yang kuat untuk pengguna tertentu dengan perintah ini:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

Untuk menonaktifkan kata sandi yang kuat untuk semua pengguna, gunakan:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [Informasi selengkapnya tentang kebijakan kata sandi](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Cara menyambungkan ke Microsoft 365 dengan PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Informasi selengkapnya tentang perintah PowerShell MsolUser](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
