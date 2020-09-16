---
title: Masalah dengan MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755134"
---
# <a name="issues-with-azure-mfa"></a>Masalah dengan Azure MFA
Ada beberapa hal untuk diperiksa jika pengguna tidak bisa masuk menggunakan multi-Factor Authentication (MFA)

1. Pengguna yang terpengaruh mungkin diblokir di portal Azure Active Directory. Jika demikian, upaya autentikasi untuk pengguna tertentu tersebut akan secara otomatis ditolak. [Ikuti langkah-langkah dalam artikel ini untuk membuka blokir.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Jika membuka blokir pengguna tidak membantu atau pengguna tidak diblokir, Anda bisa mencoba mengatur ulang MFA untuk pengguna dan mereka akan melewati proses pendaftaran lagi. [Ikuti langkah-langkah di artikel ini.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Jika ini pertama kalinya Anda mengaktifkan MFA dan pengguna Anda tidak dapat masuk ke klien non-browser seperti Outlook, Skype, dll, mungkin ADAL (pustaka autentikasi direktori aktif) tidak diaktifkan pada langganan O365 Anda. Dalam kasus ini, Anda perlu menyambungkan ke Exchange Online PowerShell dan menjalankan cmdlet ini:  *set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*