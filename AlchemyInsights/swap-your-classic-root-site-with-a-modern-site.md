---
title: Menukar situs akar klasik Anda dengan situs modern
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691182"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="460eb-102">Menukar situs akar klasik Anda dengan situs modern</span><span class="sxs-lookup"><span data-stu-id="460eb-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="460eb-103">Jika lingkungan Anda disiapkan sebelum 2019 April, Anda bisa mengubah situs akar Anda menjadi situs modern dengan menggunakan Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="460eb-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="460eb-104">Jika Anda memiliki situs yang berbeda yang ingin Anda gunakan sebagai situs akar Anda, Anda bisa mengganti [(bertukar) situs akar](https://docs.microsoft.com/sharepoint/modern-root-site) dengan file tersebut.</span><span class="sxs-lookup"><span data-stu-id="460eb-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="460eb-105">Gunakan [invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) untuk menukar lokasi situs dengan situs lain saat mengarsipkan situs asli.</span><span class="sxs-lookup"><span data-stu-id="460eb-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="460eb-106">Tersedia untuk kedua situs tim (tidak tersambung ke grup) dan situs komunikasi.</span><span class="sxs-lookup"><span data-stu-id="460eb-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="460eb-107">Kemampuan tambahan akan segera diperkenalkan yang akan memungkinkan Anda untuk tetap menggunakan konten di situs, tapi mengonversi situs yang sudah ada ke situs komunikasi.</span><span class="sxs-lookup"><span data-stu-id="460eb-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="460eb-108">Kapabilitas ini akan diluncurkan secara bertahap.</span><span class="sxs-lookup"><span data-stu-id="460eb-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="460eb-109">Lanjutkan untuk memeriksa pusat pesan untuk pembaruan.</span><span class="sxs-lookup"><span data-stu-id="460eb-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="460eb-110">Masalah yang diketahui dengan situs bertukar</span><span class="sxs-lookup"><span data-stu-id="460eb-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="460eb-111">Situs target mungkin mengembalikan kesalahan "tidak ditemukan" (HTTP 404) untuk periode waktu yang singkat.</span><span class="sxs-lookup"><span data-stu-id="460eb-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="460eb-112">Konten harus diberi kembali untuk memperbarui indeks pencarian.</span><span class="sxs-lookup"><span data-stu-id="460eb-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="460eb-113">Tidak diperlukan langkah manual-ini akan dilakukan secara otomatis.</span><span class="sxs-lookup"><span data-stu-id="460eb-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="460eb-114">Apa pun yang bergantung pada tautan "statis" (seperti file sinkronisasi file dan OneNote) perlu dikoreksi secara manual.</span><span class="sxs-lookup"><span data-stu-id="460eb-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="460eb-115">Jika situs sumber merupakan situs berita organisasi, perbarui URL.</span><span class="sxs-lookup"><span data-stu-id="460eb-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="460eb-116">Dapatkan daftar semua situs berita organisasi.</span><span class="sxs-lookup"><span data-stu-id="460eb-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="460eb-117">Situs Project Server mungkin perlu divalidasi untuk memastikan bahwa situs tersebut masih terkait dengan benar.</span><span class="sxs-lookup"><span data-stu-id="460eb-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
