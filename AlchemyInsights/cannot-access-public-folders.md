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
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959498"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="ffb5c-102">Outlook tidak dapat menyambung ke folder publik</span><span class="sxs-lookup"><span data-stu-id="ffb5c-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="ffb5c-103">Jika akses folder publik tidak bekerja untuk beberapa pengguna, cobalah berikut ini:</span><span class="sxs-lookup"><span data-stu-id="ffb5c-103">If public folder access isn't working for few users, try the following:</span></span>

<span data-ttu-id="ffb5c-104">Menyambung ke EXO PowerShell, dan mengkonfigurasi DefaultPublicFolderMailbox pada account pengguna masalah untuk mencocokkan satu pada akun pengguna bekerja.</span><span class="sxs-lookup"><span data-stu-id="ffb5c-104">Connect to EXO PowerShell, and configure the DefaultPublicFolderMailbox on the problem user account to match one on a working user account.</span></span>

<span data-ttu-id="ffb5c-105">Contoh:</span><span class="sxs-lookup"><span data-stu-id="ffb5c-105">Example:</span></span>

<span data-ttu-id="ffb5c-106">Get-kotak surat WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="ffb5c-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="ffb5c-107">Set-kotak surat ProblemUser-DefaultPublicFolderMailbox \<nilai dari perintah sebelumnya></span><span class="sxs-lookup"><span data-stu-id="ffb5c-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="ffb5c-108">Tunggu setidaknya satu jam agar perubahan diterapkan.</span><span class="sxs-lookup"><span data-stu-id="ffb5c-108">Wait at least one hour for the change to take effect.</span></span>