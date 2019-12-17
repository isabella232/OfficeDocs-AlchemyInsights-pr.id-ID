---
title: Cari di SharePoint online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c4ff98f0cf928834c803542340b32da15a40d583
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/15/2019
ms.locfileid: "40044046"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="018b7-102">Konten merangkak dan indeks di SharePoint online</span><span class="sxs-lookup"><span data-stu-id="018b7-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="018b7-103">Konten harus dirayapi dan ditambahkan ke indeks pencarian bagi pengguna untuk menemukan apa yang mereka Cari di SharePoint online.</span><span class="sxs-lookup"><span data-stu-id="018b7-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="018b7-104">Konten secara otomatis dirayapi berdasarkan jadwal perayapan yang telah ditetapkan sebelumnya (jadwal perayapan tidak dapat diubah).</span><span class="sxs-lookup"><span data-stu-id="018b7-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="018b7-105">Crawler mengambil konten yang telah berubah sejak Crawl terakhir dan memperbarui indeks.</span><span class="sxs-lookup"><span data-stu-id="018b7-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="018b7-106">Untuk memastikan konten dirayapi dan indeks diperbarui, Perhatikan hal berikut:</span><span class="sxs-lookup"><span data-stu-id="018b7-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="018b7-107">Pastikan konten dapat ditemukan dengan [membuat konten situs dicari](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="018b7-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="018b7-108">Bila Anda telah mengubah properti terkelola, atau bila Anda telah mengubah pemetaan properti yang dirayapi dan terkelola, situs harus dirayapi ulang sebelum perubahan Anda akan terlihat di indeks penelusuran.</span><span class="sxs-lookup"><span data-stu-id="018b7-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="018b7-109">Karena perubahan yang dibuat di skema pencarian, dan bukan ke situs aktual, perayap tidak akan secara otomatis mengindeks ulang situs.</span><span class="sxs-lookup"><span data-stu-id="018b7-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="018b7-110">Untuk info selengkapnya, lihat [secara manual meminta perayapan dan mengindeks ulang situs, Perpustakaan, atau daftar](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="018b7-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="018b7-111">Tunggu minimal 24 jam setelah meminta perayapan dan indeks ulang penuh secara manual untuk mengetahui apakah Anda masih mengalami masalah.</span><span class="sxs-lookup"><span data-stu-id="018b7-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="018b7-112">Jika lebih dari 24 jam telah berlalu sejak Anda memulai Crawl dan Full Re-index, silakan log kasus dukungan.</span><span class="sxs-lookup"><span data-stu-id="018b7-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="018b7-113">Dalam banyak kasus, kami telah bekerja pada solusi.</span><span class="sxs-lookup"><span data-stu-id="018b7-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="018b7-114">Tolong beri kami setidaknya 24 jam untuk menyelesaikan solusi.</span><span class="sxs-lookup"><span data-stu-id="018b7-114">Please give us at least 24 hours to complete a solution.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="018b7-115">Jika situs, dokumen (Perpustakaan), atau daftar telah dihapus dan masih menunjukkan di hasil pencarian, pengguna akan menerima **galat 404 file tidak ditemukan** ketika mencoba untuk mengaksesnya.</span><span class="sxs-lookup"><span data-stu-id="018b7-115">If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="018b7-116">Masalah ini harus dicatat sebagai kasus dukungan untuk penyelidikan lebih lanjut.</span><span class="sxs-lookup"><span data-stu-id="018b7-116">This issue should be logged as a support case for further investigation.</span></span> 



