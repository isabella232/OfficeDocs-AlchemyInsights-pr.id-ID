---
title: Pemecahan masalah ediscovery menyimpan kesalahan
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676152"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a><span data-ttu-id="d1952-102">Pemecahan masalah ediscovery menyimpan kesalahan</span><span class="sxs-lookup"><span data-stu-id="d1952-102">Troubleshooting ediscovery holds errors</span></span>

<span data-ttu-id="d1952-103">Mengalami masalah dengan eDiscovery yang dialami?</span><span class="sxs-lookup"><span data-stu-id="d1952-103">Experiencing issues with eDiscovery holds?</span></span> <span data-ttu-id="d1952-104">Berikut beberapa praktik terbaik untuk dipertimbangkan:</span><span class="sxs-lookup"><span data-stu-id="d1952-104">Here are some best practices to consider:</span></span>

- <span data-ttu-id="d1952-105">Periksa status distribusi tahan.</span><span class="sxs-lookup"><span data-stu-id="d1952-105">Check the hold distribution status.</span></span>  <span data-ttu-id="d1952-106">Jika status Aktif **(Tertunda)** atau **Nonaktif (Tertunda),** tunggu hingga pendistribusian penangguhan selesai.</span><span class="sxs-lookup"><span data-stu-id="d1952-106">If status is **On (Pending)** or **Off (Pending)**, wait for hold distribution to complete.</span></span>
- <span data-ttu-id="d1952-107">Gabungkan eDiscovery menyimpan pembaruan ke dalam satu permintaan massal daripada memperbarui kebijakan berulang kali untuk setiap transaksi.</span><span class="sxs-lookup"><span data-stu-id="d1952-107">Merge eDiscovery hold updates into a single bulk request instead of updating the policy repeatedly for each transaction.</span></span>
- <span data-ttu-id="d1952-108">Jalankan Set-CaseHoldPolicy <policyname> -RetryDistribution di Powershell Pusat Keamanan dan Kepatuhan.</span><span class="sxs-lookup"><span data-stu-id="d1952-108">Run Set-CaseHoldPolicy <policyname> -RetryDistribution in the Security and Compliance Center Powershell.</span></span> <span data-ttu-id="d1952-109">Untuk detailnya, [lihat Koneksi pusat & PowerShell Pusat Kepatuhan](/powershell/exchange/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="d1952-109">For details, see [Connect to Security & Compliance Center PowerShell](/powershell/exchange/connect-to-scc-powershell).</span></span>

<span data-ttu-id="d1952-110">Untuk langkah-langkah dalam memeriksa pengaturan ini dan praktik terbaik tambahan untuk mengurangi dan mengatasi masalah menyelenggarakan eDiscovery, lihat Memecahkan masalah [kesalahan tahan eDiscovery.](/microsoft-365/compliance/hold-distribution-errors)</span><span class="sxs-lookup"><span data-stu-id="d1952-110">For steps to check these settings and additional best practices for mitigating and resolving eDiscovery holds issues, see [Troubleshoot eDiscovery hold errors](/microsoft-365/compliance/hold-distribution-errors).</span></span>
<span data-ttu-id="d1952-111">Untuk informasi tentang pemecahan masalah eDiscovery umum lainnya, lihat [Selidiki, memecahkan masalah, dan mengatasi masalah eDiscovery umum.](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)</span><span class="sxs-lookup"><span data-stu-id="d1952-111">For info about troubleshooting other common eDiscovery issues, see [Investigate, troubleshoot, and resolve common eDiscovery issues](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span></span>
