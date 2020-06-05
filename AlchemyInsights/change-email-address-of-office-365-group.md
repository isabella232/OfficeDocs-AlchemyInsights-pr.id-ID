---
title: Ubah Alamat email dari Microsoft 365 grup
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
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580660"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="b8158-102">Ubah Alamat email dari Microsoft 365 grup</span><span class="sxs-lookup"><span data-stu-id="b8158-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="b8158-103">Anda dapat mengubah alamat email dari Microsoft 365 grup dengan menggunakan pusat admin.</span><span class="sxs-lookup"><span data-stu-id="b8158-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="b8158-104">Cukup pilih grup dan pilih @edit alamat email.</span><span class="sxs-lookup"><span data-stu-id="b8158-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="b8158-105">Anda juga dapat menggunakan perintah EXO PowerShell untuk mengubah alamat SMTP primer Microsoft 365 grup:</span><span class="sxs-lookup"><span data-stu-id="b8158-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="b8158-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="b8158-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="b8158-107">Contoh:</span><span class="sxs-lookup"><span data-stu-id="b8158-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
