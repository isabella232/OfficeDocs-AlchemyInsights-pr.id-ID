---
title: Tidak dapat mengakses folder publik
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891752"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="12e23-102">Outlook tidak dapat menyambung ke folder publik</span><span class="sxs-lookup"><span data-stu-id="12e23-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="12e23-103">Jika akses folder publik tidak bekerja untuk beberapa pengguna, cobalah berikut ini:</span><span class="sxs-lookup"><span data-stu-id="12e23-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="12e23-104">Sambungkan ke EXO PowerShell dan konfigurasikan parameter DefaultPublicFolderMailbox pada account pengguna masalah untuk mencocokkan parameter pada akun pengguna bekerja.</span><span class="sxs-lookup"><span data-stu-id="12e23-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="12e23-105">Contoh:</span><span class="sxs-lookup"><span data-stu-id="12e23-105">Example:</span></span>

<span data-ttu-id="12e23-106">Get-kotak surat WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="12e23-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="12e23-107">Set-kotak surat ProblemUser-DefaultPublicFolderMailbox \<nilai dari perintah sebelumnya></span><span class="sxs-lookup"><span data-stu-id="12e23-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="12e23-108">Tunggu setidaknya satu jam agar perubahan diterapkan.</span><span class="sxs-lookup"><span data-stu-id="12e23-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="12e23-109">Jika masalah tetap ada, ikuti [prosedur ini](https://aka.ms/pfcte) untuk memecahkan masalah akses folder publik menggunakan Outlook.</span><span class="sxs-lookup"><span data-stu-id="12e23-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>