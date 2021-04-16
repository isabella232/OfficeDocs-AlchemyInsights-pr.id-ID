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
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810487"
---
# <a name="issues-with-azure-mfa"></a>Masalah dengan Azure MFA
Terdapat beberapa hal yang perlu diperiksa jika pengguna tidak dapat masuk menggunakan multi-factor authentication (MFA)

1. Pengguna yang terpengaruh mungkin diblokir dalam Portal Azure Active Directory. Jika demikian, Percobaan autentikasi untuk pengguna tertentu tersebut akan otomatis ditolak. [Ikuti langkah-langkah dalam artikel ini untuk membuka blokirnya.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Jika membuka blokir pengguna tidak membantu atau pengguna tidak diblokir, Anda dapat mencoba mereset MFA untuk pengguna tersebut dan mereka akan melalui proses pendaftaran lagi. [Ikuti langkah-langkah dalam artikel ini.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Jika ini adalah kali pertama Anda mengaktifkan MFA dan pengguna tidak dapat masuk ke klien non-browser seperti Outlook, Skype, dll, mungkin ADAL (Pustaka Autentikasi Direktori Aktif) tidak diaktifkan pada langganan O365 Anda. Dalam hal ini, Anda perlu menyambungkan ke Exchange Online Powershell dan menjalankan cmdlet ini:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*