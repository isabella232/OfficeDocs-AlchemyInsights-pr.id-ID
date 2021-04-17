---
title: Mengubah alamat email grup Microsoft 365 atau Microsoft Teams
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
- "4704"
ms.openlocfilehash: 7800a447c5dfcc8397121e1149921916ff7944ac
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819083"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a><span data-ttu-id="541b3-102">Mengubah alamat email grup Microsoft 365 atau Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="541b3-102">Change email address of a Microsoft 365 group or Microsoft Teams</span></span>

<span data-ttu-id="541b3-103">Anda dapat mengubah alamat email grup Microsoft 365 atau Microsoft Teams menggunakan [pusat admin Microsoft 365](https://admin.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="541b3-103">You can change the email address of a Microsoft 365 group or Microsoft Teams by using the [Microsoft 365 admin center](https://admin.microsoft.com/).</span></span> <span data-ttu-id="541b3-104">Cukup pilih grup lalu pilih @edit alamat email.</span><span class="sxs-lookup"><span data-stu-id="541b3-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="541b3-105">Anda juga dapat menggunakan perintah EXO PowerShell berikut untuk mengubah alamat SMTP utama grup Microsoft 365/Teams:</span><span class="sxs-lookup"><span data-stu-id="541b3-105">You can also use the following EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group/Teams:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="541b3-106">Contoh:</span><span class="sxs-lookup"><span data-stu-id="541b3-106">Example:</span></span>

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
