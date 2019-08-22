---
title: Perubahan sandi kuat persyaratan
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
ms.openlocfilehash: f8790a26ec7c5de57f5dbfc9e1c162767c599f03
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36518762"
---
# <a name="change-strong-password-requirement"></a>Perubahan sandi kuat persyaratan

Microsoft memerlukan sandi yang kuat secara default. 

Menggunakan PowerShell, Anda dapat menonaktifkan sandi yang kuat untuk pengguna tertentu dengan perintah ini:<br>
*Set-MsolUser-UserPrincipalName <UserPrincipalName> -StrongPasswordRequired $false*

- [Informasi lebih lanjut tentang kebijakan password](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Cara menyambung ke Office 365 dengan PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Informasi lebih lanjut tentang PowerShell MsolUser perintah](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)