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
# <a name="issues-with-azure-mfa"></a>Masalah dengan Azure MFA
Ada beberapa hal untuk memeriksa apakah pengguna tidak dapat masuk menggunakan otentikasi multi faktor (MFA)

1. Pengguna yang dipakai mungkin diblokir di Azure Active Directory portal. Jika itu terjadi, otentikasi upaya untuk pengguna khusus tersebut akan secara otomatis ditolak. [Silakan ikuti langkah di artikel ini untuk membukanya.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Jika blokir pengguna tidak membantu atau pengguna tidak diblokir Anda dapat mencoba untuk me-reset MFA untuk pengguna dan mereka akan melalui proses mendaftar lagi. [Silakan ikuti langkah di artikel ini.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Jika ini adalah pertama kalinya Anda mengaktifkan MFA dan pengguna tidak dapat login ke klien non-browser seperti Outlook, Skype, dll, mungkin ADAL (Active Directory Authentication Library) tidak diaktifkan pada langganan O365 Anda. Dalam hal ini Anda akan perlu untuk terhubung ke Exchange Online PowerShell dan menjalankan cmdlet ini:  *set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*