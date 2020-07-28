---
title: Tidak dapat mengubah nama pengguna
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439549"
---
# <a name="unable-to-change-username"></a><span data-ttu-id="c2c5c-102">Tidak dapat mengubah nama pengguna</span><span class="sxs-lookup"><span data-stu-id="c2c5c-102">Unable to change UserName</span></span>

<span data-ttu-id="c2c5c-103">Dalam beberapa kasus, perubahan UPN (UserPrincipalName) tidak disebarkan ke Cloud.</span><span class="sxs-lookup"><span data-stu-id="c2c5c-103">In some cases, UPN (UserPrincipalName) changes aren't propagated to the cloud.</span></span> <span data-ttu-id="c2c5c-104">Anda mungkin menerima galat validasi di portal 365 Office atau tidak dapat mengubah nama pengguna atau alamat email.</span><span class="sxs-lookup"><span data-stu-id="c2c5c-104">You might receive validation errors in the Office 365 portal or be unable to change the username or email address.</span></span> <span data-ttu-id="c2c5c-105">Untuk mengatasi masalah ini, secara manual menetapkan UserPrincipalName menggunakan perintah PowerShell ini.</span><span class="sxs-lookup"><span data-stu-id="c2c5c-105">To resolve this issue, manually set UserPrincipalName using this PowerShell command.</span></span>

<span data-ttu-id="c2c5c-106">**Contoh: mengubah nama pengguna**</span><span class="sxs-lookup"><span data-stu-id="c2c5c-106">**Example: Rename a user**</span></span>

<span data-ttu-id="c2c5c-107">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="c2c5c-107">PowerShellCopy</span></span>

<span data-ttu-id="c2c5c-108">PS C: \> set-MsolUserPrincipalName-UserPrincipalName "davidc@contoso.com"-NewUserPrincipalName "davidchew@contoso.com"</span><span class="sxs-lookup"><span data-stu-id="c2c5c-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span></span>

<span data-ttu-id="c2c5c-109">Perintah ini mengganti nama davidc@contoso.com menjadi davidchew@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="c2c5c-109">This command renames davidc@contoso.com to davidchew@contoso.com.</span></span>

<span data-ttu-id="c2c5c-110">Untuk informasi selengkapnya, lihat [set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span><span class="sxs-lookup"><span data-stu-id="c2c5c-110">For more information, see [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span></span>