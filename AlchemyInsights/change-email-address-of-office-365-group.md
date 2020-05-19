---
title: Mengubah alamat email dari Microsoft 365 grup
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
- "4704"
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/27/2020
ms.locfileid: "44282926"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a><span data-ttu-id="22153-102">Mengubah alamat email dari Microsoft 365 grup</span><span class="sxs-lookup"><span data-stu-id="22153-102">Change email address of an Microsoft 365 group</span></span>

<span data-ttu-id="22153-103">Anda dapat mengubah alamat email dari Microsoft 365 grup dengan menggunakan pusat admin.</span><span class="sxs-lookup"><span data-stu-id="22153-103">You can change the email address of an Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="22153-104">Cukup pilih grup dan pilih @edit alamat email.</span><span class="sxs-lookup"><span data-stu-id="22153-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="22153-105">Anda juga dapat menggunakan perintah EXO PowerShell untuk mengubah alamat SMTP primer Microsoft 365 grup:</span><span class="sxs-lookup"><span data-stu-id="22153-105">You can also use following the EXO PowerShell command to change the primary SMTP address of an Microsoft 365 group:</span></span>

<span data-ttu-id="22153-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="22153-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="22153-107">Contoh:</span><span class="sxs-lookup"><span data-stu-id="22153-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
