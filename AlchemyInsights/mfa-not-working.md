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
ms.openlocfilehash: 276f6b2212c9d85df726cb46a46dee7828b34c89
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/18/2019
ms.locfileid: "36545172"
---
# <a name="issues-with-mfa"></a>Masalah dengan MFA
Ada beberapa hal untuk memeriksa apakah pengguna tidak dapat login menggunakan otentikasi multi faktor (MFA)

1. Pengguna yang dipakai mungkin diblokir di Azure Active Directory portal. Jika itu terjadi, otentikasi upaya untuk pengguna khusus tersebut akan secara otomatis ditolak. [Silakan ikuti langkah di artikel ini untuk membukanya.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Jika blokir pengguna tidak membantu atau pengguna tidak diblokir Anda dapat mencoba untuk me-reset MFA untuk pengguna dan mereka akan melalui proses mendaftar lagi. [Silakan ikuti langkah di artikel ini.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Jika ini adalah pertama kalinya Anda mengaktifkan MFA dan pengguna tidak dapat login ke klien non-browser seperti Outlook, Skype, dll, mungkin ADAL (Active Directory Authentication Library) tidak diaktifkan pada langganan O365 Anda. Dalam hal ini Anda akan perlu untuk terhubung ke Exchange Online PowerShell dan menjalankan cmdlet ini:  *set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*