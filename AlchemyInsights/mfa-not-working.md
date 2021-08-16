---
title: Masalah dengan MFA
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: b39c79063c66ea41585c8f9eec372bfac77bc0aa29ded5a5572e06c141b28f80
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098605"
---
# <a name="issues-with-azure-mfa"></a>Masalah dengan Azure MFA
Terdapat beberapa hal yang perlu diperiksa jika pengguna tidak dapat masuk menggunakan multi-factor authentication (MFA)

1. Pengguna yang terpengaruh mungkin diblokir di Azure Active Directory Portal. Jika demikian, Percobaan autentikasi untuk pengguna tertentu tersebut akan otomatis ditolak. [Ikuti langkah-langkah dalam artikel ini untuk membuka blokirnya.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Jika membuka blokir pengguna tidak membantu atau pengguna tidak diblokir, Anda dapat mencoba mereset MFA untuk pengguna tersebut dan mereka akan melalui proses pendaftaran lagi. [Ikuti langkah-langkah dalam artikel ini.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Jika ini adalah kali pertama Anda mengaktifkan MFA dan pengguna tidak dapat masuk ke klien non-browser seperti Outlook, Skype, dll, mungkin ADAL (Pustaka Autentikasi Direktori Aktif) tidak diaktifkan pada langganan O365 Anda. Dalam hal ini, Anda perlu menyambungkan ke Exchange Online Powershell dan menjalankan cmdlet ini: *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*