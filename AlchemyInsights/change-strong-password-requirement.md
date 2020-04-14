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
ms.openlocfilehash: 21f80a7cc8b00ac56acdb05add1e1bfdfac9d827
ms.sourcegitcommit: c061f1dfa6f557a9ec083dd030b73b121d9864ea
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/14/2020
ms.locfileid: "43286266"
---
# <a name="change-strong-password-requirement"></a>Mengubah persyaratan sandi yang kuat

Microsoft memerlukan sandi yang kuat secara default. 

Dengan menggunakan PowerShell, Anda dapat menonaktifkan sandi yang kuat untuk pengguna tertentu dengan perintah ini:<br>
*Set-MsolUser-UserPrincipalName <UserPrincipalName> -strongpasswordrequired $false*

- [Informasi lebih lanjut tentang kebijakan sandi](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Cara menyambung ke Office 365 dengan PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Informasi lebih lanjut tentang perintah PowerShell MsolUser](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
- [Menetapkan sandi pengguna individu agar tidak pernah kedaluwarsa](https://docs.microsoft.com/microsoft-365/admin/add-users/set-password-to-never-expire)
