---
title: Perubahan sandi kuat persyaratan
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: 53affd2a347c004e7b21b353c2b3df98bc30a585
ms.sourcegitcommit: a7e5ca472000dfec471950bafd12eee8d7144f74
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/16/2019
ms.locfileid: "35701587"
---
# <a name="change-strong-password-requirement"></a>Perubahan sandi kuat persyaratan

Sandi yang kuat diperlukan secara default. 

Menggunakan PowerShell Anda dapat menonaktifkan sandi yang kuat untuk pengguna tertentu dengan perintah ini:<br>
*Set-MsolUser-UserPrincipalName <UserPrincipalName> -StrongPasswordRequired $false*

- [Informasi lebih lanjut tentang kebijakan password](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Bagaimana menghubungkan O365 dengan PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Informasi lebih lanjut tentang PowerShell MsolUser perintah](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)