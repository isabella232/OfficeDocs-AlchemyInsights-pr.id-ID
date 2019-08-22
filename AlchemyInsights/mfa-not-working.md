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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36545172"
---
# <a name="issues-with-mfa"></a>Masalah dengan MFA
Ada beberapa hal untuk memeriksa jika pengguna tidak dapat login menggunakan multi faktor otentikasi (MFA)

1. Terkena pengguna dapat diblokir di Azure Portal direktori aktif. Jika itu terjadi, otentikasi upaya untuk itu pengguna akan secara otomatis ditolak. [Ikuti langkah-langkah dalam artikel ini untuk mereka.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Jika blokir pengguna tidak membantu atau pengguna tidak diblokir Anda dapat mencoba untuk me-reset MFA untuk pengguna dan mereka akan pergi melalui proses pendaftaran lagi. [Ikuti langkah-langkah dalam artikel ini.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Jika ini adalah pertama kali Anda diaktifkan MFA dan pengguna tidak dapat login untuk klien bebas-browser seperti Outlook, Skype, dll, mungkin ADAL (Active Directory otentikasi Perpustakaan) tidak diaktifkan pada kepelangganan O365. Dalam hal ini Anda akan perlu untuk menyambung ke Exchange Online Powershell dan menjalankan cmdlet ini:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*