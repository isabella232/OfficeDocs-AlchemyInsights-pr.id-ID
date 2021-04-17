---
title: Pesan selamat datang di Grup Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "5685"
ms.openlocfilehash: 6c46ba1b2c2c94e21d7c76e45df1d416ba423faf
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806409"
---
# <a name="welcome-message-in-microsoft-365-groups"></a><span data-ttu-id="51380-102">Pesan selamat datang di Grup Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="51380-102">Welcome message in Microsoft 365 Groups</span></span>

<span data-ttu-id="51380-103">Pengguna baru yang bergabung dengan grup Microsoft 365 akan menerima email selamat datang jika properti "UnifiedGroupWelcomePesanEnabled" diatur ke True.</span><span class="sxs-lookup"><span data-stu-id="51380-103">New users joining Microsoft 365 group will receive welcome email if the "UnifiedGroupWelcomeMessageEnabled" property is True.</span></span>

<span data-ttu-id="51380-104">Jika Anda ingin menonaktifkan pesan selamat datang, gunakan perintah [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) berikut:</span><span class="sxs-lookup"><span data-stu-id="51380-104">In case you want to disable the welcome message, use the following [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) command:</span></span>

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
