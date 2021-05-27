---
title: Inventaris perangkat lunak hilang atau tidak akurat
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/26/2021
ms.locfileid: "52676518"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a><span data-ttu-id="d04f9-102">Inventaris perangkat lunak hilang atau tidak akurat</span><span class="sxs-lookup"><span data-stu-id="d04f9-102">Software inventory is missing or inaccurate</span></span>

<span data-ttu-id="d04f9-103">Inventaris perangkat lunak di Pengelolaan Ancaman dan Kerentanan (TVM) adalah daftar perangkat lunak yang dikenal di organisasi Anda dengan Common Platform Enumerations (CPE) resmi.</span><span class="sxs-lookup"><span data-stu-id="d04f9-103">The software inventory in threat and vulnerability management (TVM) is a list of known software in your organization with official Common Platform Enumerations (CPE).</span></span>

<span data-ttu-id="d04f9-104">Produk perangkat lunak tanpa CPE resmi tidak memiliki kerentanan yang diterbitkan.</span><span class="sxs-lookup"><span data-stu-id="d04f9-104">Software products without an official CPE don’t have vulnerabilities published.</span></span> <span data-ttu-id="d04f9-105">Inventaris juga menyertakan detail seperti nama vendor, jumlah item, ancaman, dan jumlah perangkat yang diekspos.</span><span class="sxs-lookup"><span data-stu-id="d04f9-105">The inventory also includes details such as the name of the vendor, number of weaknesses, threats, and number of exposed devices.</span></span>

<span data-ttu-id="d04f9-106">Perubahan perangkat lunak pada perangkat biasanya terlihat di portal keamanan dalam waktu dua jam.</span><span class="sxs-lookup"><span data-stu-id="d04f9-106">Software changes on devices are typically reflected in security portals within two hours.</span></span> <span data-ttu-id="d04f9-107">Namun, terkadang membutuhkan waktu lebih lama.</span><span class="sxs-lookup"><span data-stu-id="d04f9-107">However, it may sometimes take longer.</span></span> <span data-ttu-id="d04f9-108">Saat ini, sinkronisasi belum dapat dilakukan; ini adalah penilaian berkelanjutan yang sedang berlangsung.</span><span class="sxs-lookup"><span data-stu-id="d04f9-108">There’s currently no way to force a sync; this is an ongoing continuous assessment.</span></span>

<span data-ttu-id="d04f9-109">Jika Anda membuat perubahan perangkat lunak dan perubahan tersebut tidak secara akurat terlihat di TVM setelah 5 jam, ikuti langkah-langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="d04f9-109">If you made a software change and the change is not accurately reflected in TVM after 5 hours, follow these steps:</span></span>

1. <span data-ttu-id="d04f9-110">Periksa bagian bukti perangkat lunak untuk memahami bagaimana perangkat lunak terdeteksi.</span><span class="sxs-lookup"><span data-stu-id="d04f9-110">Check the software evidence section to understand how the software was detected.</span></span>
1. <span data-ttu-id="d04f9-111">Pastikan bahwa perangkat lunak ini didukung.</span><span class="sxs-lookup"><span data-stu-id="d04f9-111">Make sure that the software is supported.</span></span> <span data-ttu-id="d04f9-112">Perangkat lunak mungkin hanya terlihat di tingkat perangkat meskipun saat ini tidak didukung oleh Pengelolaan Ancaman dan Kerentanan.</span><span class="sxs-lookup"><span data-stu-id="d04f9-112">Software may be visible only at the device level even if it is currently not supported by threat and vulnerability management.</span></span> <span data-ttu-id="d04f9-113">Namun, hanya data terbatas yang tersedia.</span><span class="sxs-lookup"><span data-stu-id="d04f9-113">However, only limited data is available.</span></span>
1. <span data-ttu-id="d04f9-114">Untuk langkah-langkah melaporkan ketidakakuratan dari portal, lihat [Melaporkan ketidakakuratan](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span><span class="sxs-lookup"><span data-stu-id="d04f9-114">For steps to report the inaccuracy from the portal, see [Report inaccuracy](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span></span>
   
    <span data-ttu-id="d04f9-115">**Catatan**: Melaporkan ketidakakuratan dari portal MDE adalah saluran satu arah yang harus di engineering.</span><span class="sxs-lookup"><span data-stu-id="d04f9-115">**Note**: Reporting an inaccuracy from the MDE portal is a one-way channel to engineering.</span></span> <span data-ttu-id="d04f9-116">Jika masalah mendesak, buka tiket dukungan.</span><span class="sxs-lookup"><span data-stu-id="d04f9-116">If the issue is urgent, open a support ticket.</span></span>

<span data-ttu-id="d04f9-117">Untuk informasi selengkapnya, lihat [Inventaris perangkat lunak - Pengelolaan Ancaman dan Kerentanan](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span><span class="sxs-lookup"><span data-stu-id="d04f9-117">For more information, see [Software inventory - threat and vulnerability management](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span></span>