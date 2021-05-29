---
title: Penundaan atau pembatasan mikro di Exchange Online PowerShell
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
- "3500011"
- "5106"
ms.openlocfilehash: 204e0248bc2f07f14fa789d1d2999495910ee034
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702129"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="e8fda-102">Penundaan atau pembatasan mikro di Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="e8fda-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="e8fda-103">Anda mungkin melihat peringatan "Keterlambatan mikro diterapkan" atau keterlambatan ketika menjalankan skrip dan cmdlet di Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="e8fda-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="e8fda-104">Berikut beberapa saran untuk mengatasi masalah ini:</span><span class="sxs-lookup"><span data-stu-id="e8fda-104">Here are a few suggestions how to solve this:</span></span>

- <span data-ttu-id="e8fda-105">Jalankan diagnostik kami untuk blak-atik kebijakan pembatasan PowerShell penyewa Anda.</span><span class="sxs-lookup"><span data-stu-id="e8fda-105">Please run our diagnostics to relax your tenant's PowerShell throttling policies.</span></span> <span data-ttu-id="e8fda-106">Solusi ini akan menyelesaikan masalah sebagian besar.</span><span class="sxs-lookup"><span data-stu-id="e8fda-106">This solution will solve the problem for most.</span></span>
- <span data-ttu-id="e8fda-107">Jika masalah masih belum diatasi, gunakan modul [PowerShell Exchange Online v2,](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)yang menyertakan CMDlets yang didasarkan pada REST API dan secara signifikan lebih banyak melakukan.</span><span class="sxs-lookup"><span data-stu-id="e8fda-107">If issue still not solved, use the [Exchange Online v2 PowerShell module](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="e8fda-108">Ini dapat menjadi solusi yang baik untuk banyak Get- CMDlet yang sering digunakan.</span><span class="sxs-lookup"><span data-stu-id="e8fda-108">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="e8fda-109">Jika anda perlu menggunakan CMDlets yang tidak tercakup dalam modul v2, silakan lihat Menjalankan [cmdlet PowerShell](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)untuk sejumlah besar pengguna di Office 365 , yang membahas tentang cara mengelilingi batas pembatasan PowerShell di Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="e8fda-109">If you need to use CMDlets that are not covered in the v2 module, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around PowerShell throttling limits in Exchange Online.</span></span>
