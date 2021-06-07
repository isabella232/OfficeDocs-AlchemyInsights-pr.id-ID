---
title: Masalah kinerja pertahanan Microsoft untuk Titik Akhir di Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794006"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="5a8f5-102">Masalah kinerja pertahanan Microsoft untuk Titik Akhir di Linux</span><span class="sxs-lookup"><span data-stu-id="5a8f5-102">Performance issues for Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="5a8f5-103">Artikel ini memandu Anda dalam langkah-langkah mengidentifikasi masalah kinerja pertahanan Microsoft untuk Titik Akhir di Linux.</span><span class="sxs-lookup"><span data-stu-id="5a8f5-103">This article guides you through the steps of identifying performance issues for Microsoft Defender for Endpoint on Linux.</span></span>

<span data-ttu-id="5a8f5-104">Penting untuk memverifikasi terlebih dahulu bahwa masalah yang Anda alami telah diatasi dengan [versi terbaru.](/microsoft-365/security/defender-endpoint/linux-whatsnew)</span><span class="sxs-lookup"><span data-stu-id="5a8f5-104">It's important to first verify that the problem you're experiencing is resolved with the [latest version](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span></span> 

<span data-ttu-id="5a8f5-105">Untuk memulai penyelidikan, lihat [Memecahkan masalah kinerja Pertahanan Microsoft untuk Titik Akhir di Linux.](/microsoft-365/security/defender-endpoint/linux-support-perf)</span><span class="sxs-lookup"><span data-stu-id="5a8f5-105">To start your investigation, see [Troubleshoot performance issues for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span></span>

## <a name="exclusions"></a><span data-ttu-id="5a8f5-106">Pengecualian</span><span class="sxs-lookup"><span data-stu-id="5a8f5-106">Exclusions</span></span>

<span data-ttu-id="5a8f5-107">Pengecualian bisa membantu mengurangi masalah kinerja.</span><span class="sxs-lookup"><span data-stu-id="5a8f5-107">Exclusions can help to mitigate performance issues.</span></span> <span data-ttu-id="5a8f5-108">Tinjau pengecualian Anda sebelum memulai sehingga setiap risiko tambahan diketahui dan didokumentasikan.</span><span class="sxs-lookup"><span data-stu-id="5a8f5-108">Review your exclusions before you begin so any additional risk is known and documented.</span></span>

<span data-ttu-id="5a8f5-109">Untuk informasi selengkapnya, [lihat Mengonfigurasi dan memvalidasi pengecualian bagi Pertahanan Microsoft untuk Titik Akhir di Linux.](/microsoft-365/security/defender-endpoint/linux-exclusions)</span><span class="sxs-lookup"><span data-stu-id="5a8f5-109">For more information, see [Configure and validate exclusions for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span></span>

<span data-ttu-id="5a8f5-110">Jika Anda memiliki beberapa file & folder untuk dikecualikan dan semuanya berada di puncak yang sama, mungkin sebaiknya jangan sertakan titik naik.</span><span class="sxs-lookup"><span data-stu-id="5a8f5-110">When you have multiple files & folders to exclude and they're all on the same mountpoint, it might be easier to exclude the mountpoint.</span></span> <span data-ttu-id="5a8f5-111">Dimulai dengan rilis Februari 101.22.80, Anda dapat tidak menyertakan seluruh puncak gunung.</span><span class="sxs-lookup"><span data-stu-id="5a8f5-111">Starting with February release 101.22.80, you can exclude an entire mountpoint.</span></span>

<span data-ttu-id="5a8f5-112">Misalnya, jika /mnt/backup adalah mountpoint, Anda dapat menambahkan /mnt/backup ke daftar pengecualian dengan menjalankan perintah ini:</span><span class="sxs-lookup"><span data-stu-id="5a8f5-112">For example, if /mnt/backup is a mountpoint, you can add /mnt/backup to the exclude list by running this command:</span></span>

`$ mdatp exclusion folder add –path /mnt/backup`

<span data-ttu-id="5a8f5-113">**Catatan**: Menambahkan pengecualian meningkatkan risiko malware yang tidak terdeteksi dan harus ditangani serta diterapkan dengan hati-hati.</span><span class="sxs-lookup"><span data-stu-id="5a8f5-113">**Note**: Adding exclusions increases the risk of malware not being detected and should be handled and implemented with care.</span></span>

## <a name="need-help"></a><span data-ttu-id="5a8f5-114">Perlu Bantuan?</span><span class="sxs-lookup"><span data-stu-id="5a8f5-114">Need Help?</span></span>

<span data-ttu-id="5a8f5-115">Untuk membantu Anda dengan cara yang paling efisien, kumpulkan data diagnostik sebelum membuka kasus dukungan.</span><span class="sxs-lookup"><span data-stu-id="5a8f5-115">To assist you in the most efficient way, collect the diagnostic data before opening a support case.</span></span>
