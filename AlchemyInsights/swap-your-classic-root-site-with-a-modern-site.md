---
title: Swap situs root Classic Anda dengan situs modern
ms.author: pebaum
author: pebaum
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: fe1f0f662c49de2bd0b5b997697c98309cb7983f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/15/2019
ms.locfileid: "40042930"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="9b71b-102">Swap situs root Classic Anda dengan situs modern</span><span class="sxs-lookup"><span data-stu-id="9b71b-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="9b71b-103">Jika lingkungan Anda diatur sebelum 2019 April, Anda dapat mengubah situs akar Anda ke situs modern dengan menggunakan Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="9b71b-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="9b71b-104">Jika Anda memiliki situs yang berbeda yang ingin Anda gunakan sebagai situs akar Anda, Anda dapat mengganti [(swap) situs akar](https://docs.microsoft.com/sharepoint/modern-root-site) dengan itu.</span><span class="sxs-lookup"><span data-stu-id="9b71b-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="9b71b-105">Gunakan [invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) untuk menukar lokasi situs dengan situs lain saat pengarsipan situs asli.</span><span class="sxs-lookup"><span data-stu-id="9b71b-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="9b71b-106">Tersedia untuk kedua tim situs (tidak terhubung ke grup) dan situs komunikasi.</span><span class="sxs-lookup"><span data-stu-id="9b71b-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="9b71b-107">Kemampuan tambahan akan diperkenalkan segera yang akan memungkinkan Anda untuk tetap menggunakan konten di situs, tetapi mengkonversi situs yang ada ke situs komunikasi.</span><span class="sxs-lookup"><span data-stu-id="9b71b-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="9b71b-108">Kemampuan ini akan diluncurkan secara bertahap.</span><span class="sxs-lookup"><span data-stu-id="9b71b-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="9b71b-109">Lanjutkan untuk memeriksa Office 365 message Center untuk pembaruan.</span><span class="sxs-lookup"><span data-stu-id="9b71b-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="9b71b-110">Masalah yang diketahui dengan swapping Sites</span><span class="sxs-lookup"><span data-stu-id="9b71b-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="9b71b-111">Situs target dapat mengembalikan galat "tidak ditemukan" (HTTP 404) untuk jangka waktu yang singkat.</span><span class="sxs-lookup"><span data-stu-id="9b71b-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="9b71b-112">Konten harus di-recrawled untuk memperbarui indeks pencarian.</span><span class="sxs-lookup"><span data-stu-id="9b71b-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="9b71b-113">Tidak ada langkah manual yang diperlukan-ini akan dilakukan secara otomatis.</span><span class="sxs-lookup"><span data-stu-id="9b71b-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="9b71b-114">Apa pun tergantung pada "statis" link (seperti file Sync dan OneNote file) harus dikoreksi secara manual.</span><span class="sxs-lookup"><span data-stu-id="9b71b-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="9b71b-115">Jika situs sumber adalah situs berita organisasi, perbarui URL.</span><span class="sxs-lookup"><span data-stu-id="9b71b-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="9b71b-116">Dapatkan daftar semua situs berita organisasi.</span><span class="sxs-lookup"><span data-stu-id="9b71b-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="9b71b-117">Proyek server situs mungkin perlu divalidasi untuk memastikan bahwa mereka masih terkait dengan benar.</span><span class="sxs-lookup"><span data-stu-id="9b71b-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





