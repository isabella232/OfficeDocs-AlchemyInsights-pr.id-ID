---
title: Menggunakan DLP dalam aturan transportasi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: 124b031e2e029b745c66a71f681f57134739eafe
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915183"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="2a444-102">Menggunakan DLP dalam aturan transportasi</span><span class="sxs-lookup"><span data-stu-id="2a444-102">Using DLP in transport rules</span></span>

<span data-ttu-id="2a444-103">Untuk mengintegrasikan Pencegahan Kehilangan Data (DLP) ke dalam transportasi yang ada, gunakan kondisi **Jika pesan berisi...Informasi Sensitif**” dalam pengaturan aturan Transportasi.</span><span class="sxs-lookup"><span data-stu-id="2a444-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="2a444-104">**Untuk detail selengkapnya, lihat:**</span><span class="sxs-lookup"><span data-stu-id="2a444-104">**For more details, see:**</span></span>

- <span data-ttu-id="2a444-105">Tipe informasi sensitif DLP terintegrasi dalam aturan transportasi: [Mengintegrasikan Aturan Informasi Sensitif](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="2a444-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="2a444-106">Anda juga dapat menguji aturan dengan atau tanpa uji kebijakan menggunakan Mode Uji pada aturan.</span><span class="sxs-lookup"><span data-stu-id="2a444-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="2a444-107">Anda harus menunggu 30 menit setelah membuat aturan sebelum mengujinya.</span><span class="sxs-lookup"><span data-stu-id="2a444-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="2a444-108">Lihat [Menguji Aturan Aliran/Transportasi Email](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="2a444-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="2a444-109">**Catatan**: Jika Anda mencoba menerapkan kebijakan DLP baru dengan aturan transportasi di EAC, gunakan [Kebijakan DLP di pusat Keamanan dan Kepatuhan](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) sebagai gantinya.</span><span class="sxs-lookup"><span data-stu-id="2a444-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
