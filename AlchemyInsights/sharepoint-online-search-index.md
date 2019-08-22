---
title: Pencarian di SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 3c3f6384172b2b4d59db6059618572db11059228
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507634"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="365f9-102">Konten menperayapan dan mengindeks dalam SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="365f9-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="365f9-103">Konten harus merangkak dan ditambahkan ke indeks pencarian bagi pengguna untuk menemukan apa yang mereka mencari di SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="365f9-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="365f9-104">Konten secara otomatis merangkak berdasarkan pada jadwal yang ditetapkan merangkak (jadwal merangkak tidak berubah).</span><span class="sxs-lookup"><span data-stu-id="365f9-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="365f9-105">Crawler mengambil konten yang telah berubah sejak terakhir merangkak dan pembaruan indeks.</span><span class="sxs-lookup"><span data-stu-id="365f9-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="365f9-106">Untuk memastikan konten merangkak dan indeks diperbarui, perhatikan yang berikut ini:</span><span class="sxs-lookup"><span data-stu-id="365f9-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="365f9-107">Pastikan konten dapat ditemukan dengan [membuat konten situs dapat dicari](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="365f9-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="365f9-108">Ketika Anda telah mengubah properti yang dikelola, atau ketika Anda telah mengubah pemetaan merangkak dan berhasil properti, situs harus kembali merangkak sebelum perubahan akan tercermin dalam indeks pencarian.</span><span class="sxs-lookup"><span data-stu-id="365f9-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="365f9-109">Karena perubahan yang dibuat pada schema Cari, dan tidak ke situs sebenarnya, crawler akan secara otomatis kembali indeks situs.</span><span class="sxs-lookup"><span data-stu-id="365f9-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="365f9-110">Untuk info lebih lanjut, lihat [manual meminta merangkak dan mengindeks ulang situs, Perpustakaan atau daftar](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="365f9-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="365f9-111">Tunggu minimal 24 jam setelah secara manual meminta merangkak dan penuh kembali indeks untuk melihat jika Anda masih mengalami masalah.</span><span class="sxs-lookup"><span data-stu-id="365f9-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="365f9-112">Jika lebih dari 24 jam telah berlalu sejak memulai merangkak dan mengindeks ulang penuh, silahkan log kasus dukungan.</span><span class="sxs-lookup"><span data-stu-id="365f9-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="365f9-113">Dalam banyak kasus, kami sudah bekerja pada sebuah solusi.</span><span class="sxs-lookup"><span data-stu-id="365f9-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="365f9-114">Mohon berikan setidaknya 24 jam untuk menyelesaikan solusi.</span><span class="sxs-lookup"><span data-stu-id="365f9-114">Please give us at least 24 hours to complete a solution.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="365f9-115">Jika sebuah situs, dokumen (Perpustakaan), atau daftar dihapus dan masih menunjukkan di hasil pencarian, pengguna akan menerima **Kesalahan 404 File tidak ditemukan** ketika mencoba untuk mengaksesnya.</span><span class="sxs-lookup"><span data-stu-id="365f9-115">If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="365f9-116">Masalah ini harus login sebagai kasus dukungan untuk investigasi lebih lanjut.</span><span class="sxs-lookup"><span data-stu-id="365f9-116">This issue should be logged as a support case for further investigation.</span></span> 



