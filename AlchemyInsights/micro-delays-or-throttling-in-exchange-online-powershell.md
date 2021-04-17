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
ms.openlocfilehash: 680df9e6e2404ff6b60b17d6ac88e202e9a7bb25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830036"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="2847e-102">Penundaan atau pembatasan mikro di Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="2847e-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="2847e-103">Anda mungkin melihat peringatan "Keterlambatan mikro diterapkan" atau keterlambatan ketika menjalankan skrip dan cmdlet di Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="2847e-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="2847e-104">Berikut ini adalah dua saran terkait hal ini:</span><span class="sxs-lookup"><span data-stu-id="2847e-104">Here are two suggestions related to this:</span></span>

- <span data-ttu-id="2847e-105">Anda mungkin ingin menggunakan [modul Exchange Online v2 PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), yang menyertakan CMDlet yang berdasarkan REST API dan secara signifikan lebih berkinerja.</span><span class="sxs-lookup"><span data-stu-id="2847e-105">You might want to try using the [Exchange Online v2 PowerShell module](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="2847e-106">Ini dapat menjadi solusi yang baik untuk banyak Get- CMDlet yang sering digunakan.</span><span class="sxs-lookup"><span data-stu-id="2847e-106">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="2847e-107">Jika Anda perlu menggunakan CMDlet yang belum tercakup dalam modul v2, lihat [Menjalankan cmdlet PowerShell untuk banyak pengguna di Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), yang membahas tentang cara mengatur batas pembatasan PowerShell di Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="2847e-107">If you need to use CMDlets that are not covered in the v2 module yet, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around expected PowerShell throttling limits in Exchange Online.</span></span>
