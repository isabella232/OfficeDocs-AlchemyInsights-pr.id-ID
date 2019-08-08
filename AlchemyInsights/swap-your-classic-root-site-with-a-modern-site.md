---
title: Swap situs akar klasik dengan sebuah situs Modern
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "2579"
- "9000687"
ms.openlocfilehash: dad7d7a52222dc09aea532714a93ca89c0d9ae19
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/07/2019
ms.locfileid: "36246005"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="7e7a2-102">Swap situs akar klasik dengan sebuah situs Modern</span><span class="sxs-lookup"><span data-stu-id="7e7a2-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="7e7a2-103">Jika lingkungan Anda mengatur sebelum April 2019, Anda dapat mengubah situs akar Anda ke situs modern dengan menggunakan Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="7e7a2-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="7e7a2-104">Jika Anda memiliki situs yang berbeda yang ingin Anda gunakan sebagai situs akar Anda, Anda dapat mengganti (swap) akar situs dengan itu.</span><span class="sxs-lookup"><span data-stu-id="7e7a2-104">If you have a different site that you want to use as your root site, you can replace (swap) the root site with it.</span></span> 
    - <span data-ttu-id="7e7a2-105">Gunakan [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) untuk menukar lokasi situs dengan situs lain sementara pengarsipan situs asli.</span><span class="sxs-lookup"><span data-stu-id="7e7a2-105">Use [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="7e7a2-106">Tersedia untuk tim situs (tidak terhubung ke grup) dan komunikasi situs.</span><span class="sxs-lookup"><span data-stu-id="7e7a2-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="7e7a2-107">Kemampuan tambahan akan diperkenalkan segera yang akan memungkinkan Anda untuk tetap menggunakan konten di situs, tetapi mengubah situs yang sudah ada ke situs komunikasi.</span><span class="sxs-lookup"><span data-stu-id="7e7a2-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="7e7a2-108">Kemampuan ini akan digulirkan secara bertahap.</span><span class="sxs-lookup"><span data-stu-id="7e7a2-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="7e7a2-109">Terus memeriksa pesan 365 kantor pusat untuk update.</span><span class="sxs-lookup"><span data-stu-id="7e7a2-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="7e7a2-110">Masalah yang dikenal dengan menukar situs</span><span class="sxs-lookup"><span data-stu-id="7e7a2-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="7e7a2-111">Situs target mungkin kembali "tidak ditemukan" kesalahan (HTTP 404) untuk periode waktu yang singkat.</span><span class="sxs-lookup"><span data-stu-id="7e7a2-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="7e7a2-112">Konten akan perlu recrawled untuk memperbarui indeks pencarian.</span><span class="sxs-lookup"><span data-stu-id="7e7a2-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="7e7a2-113">Tidak ada langkah manual yang diperlukan - ini akan dilakukan secara otomatis.</span><span class="sxs-lookup"><span data-stu-id="7e7a2-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="7e7a2-114">Apa pun yang bergantung pada "statis" link (seperti File Sync dan OneNote file) akan perlu diperbaiki secara manual.</span><span class="sxs-lookup"><span data-stu-id="7e7a2-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="7e7a2-115">Jika situs sumber situs berita organisasi, memperbarui URL.</span><span class="sxs-lookup"><span data-stu-id="7e7a2-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="7e7a2-116">Mendapatkan daftar semua situs berita organisasi.</span><span class="sxs-lookup"><span data-stu-id="7e7a2-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="7e7a2-117">Lokasi Server proyek mungkin perlu divalidasi untuk memastikan bahwa mereka masih berhubungan dengan benar.</span><span class="sxs-lookup"><span data-stu-id="7e7a2-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





