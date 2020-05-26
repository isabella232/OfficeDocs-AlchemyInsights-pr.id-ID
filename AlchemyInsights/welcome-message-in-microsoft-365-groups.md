---
title: Selamat datang pesan di Microsoft 365 grup
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "5685"
ms.openlocfilehash: d82931ae6978a09e674b00640d1dd413bcce7cfd
ms.sourcegitcommit: b196100759b29aecd62b693a2bfedbbd25a697c6
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/19/2020
ms.locfileid: "44357842"
---
# <a name="welcome-message-in-microsoft-365-groups"></a>Selamat datang pesan di Microsoft 365 grup

Pengguna baru bergabung dengan Microsoft 365 grup akan menerima email Selamat datang jika properti "UnifiedGroupWelcomeMessageEnabled" benar.

Jika Anda ingin menonaktifkan pesan pembuka, gunakan perintah [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) berikut ini:

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
