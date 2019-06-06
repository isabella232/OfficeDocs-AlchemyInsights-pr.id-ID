---
title: Mengelola pencarian kamus di SharePoint Online
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c2960093bb1cfb649c26528c9f671e6d720ff237
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/05/2019
ms.locfileid: "34736056"
---
# <a name="search-in-sharepoint-online"></a><span data-ttu-id="dc222-102">Pencarian di SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="dc222-102">Search in SharePoint Online</span></span>

<span data-ttu-id="dc222-103">Konten harus merangkak dan ditambahkan ke indeks pencarian bagi pengguna untuk menemukan apa yang mereka mencari di SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="dc222-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="dc222-104">Konten secara otomatis merangkak berdasarkan pada jadwal yang ditetapkan merangkak (jadwal merangkak tidak berubah).</span><span class="sxs-lookup"><span data-stu-id="dc222-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="dc222-105">Crawler mengambil konten yang telah berubah sejak terakhir merangkak dan pembaruan indeks.</span><span class="sxs-lookup"><span data-stu-id="dc222-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="dc222-106">Untuk memastikan konten merangkak dan indeks diperbarui, ikuti langkah berikut.</span><span class="sxs-lookup"><span data-stu-id="dc222-106">To ensure content is crawled and the index is updated, follow the steps below.</span></span>

<span data-ttu-id="dc222-107">Pastikan konten dapat ditemukan dengan membuat konten situs dapat dicari.</span><span class="sxs-lookup"><span data-stu-id="dc222-107">Make sure content can be found by making site content searchable.</span></span> <span data-ttu-id="dc222-108">Untuk info lebih lanjut, lihat [mengaktifkan konten di situs harus dicari](https://docs.microsoft.com/en-us/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="dc222-108">For more info, see [Enable content on a site to be searchable](https://docs.microsoft.com/en-us/sharepoint/make-site-content-searchable).</span></span>

<span data-ttu-id="dc222-109">Ketika Anda telah mengubah properti yang dikelola, atau ketika Anda telah mengubah pemetaan merangkak dan berhasil properti, situs harus kembali merangkak sebelum perubahan akan tercermin dalam indeks pencarian.</span><span class="sxs-lookup"><span data-stu-id="dc222-109">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

<span data-ttu-id="dc222-110">Karena perubahan yang dibuat pada schema Cari, dan tidak ke situs sebenarnya, crawler akan secara otomatis kembali indeks situs.</span><span class="sxs-lookup"><span data-stu-id="dc222-110">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

<span data-ttu-id="dc222-111">Untuk info lebih lanjut, lihat [manual meminta merangkak dan mengindeks ulang situs, Perpustakaan atau daftar](https://docs.microsoft.com/en-us/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="dc222-111">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/en-us/sharepoint/crawl-site-conten).</span></span>

 <span data-ttu-id="dc222-112">Tunggu minimal 24 jam setelah secara manual meminta merangkak dan penuh kembali indeks untuk melihat jika Anda masih mengalami masalah.</span><span class="sxs-lookup"><span data-stu-id="dc222-112">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

<span data-ttu-id="dc222-113">Jika lebih dari 24 jam telah berlalu sejak memulai merangkak dan mengindeks ulang penuh, silahkan log kasus dukungan.</span><span class="sxs-lookup"><span data-stu-id="dc222-113">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="dc222-114">Dalam banyak kasus, kami sudah bekerja pada sebuah solusi.</span><span class="sxs-lookup"><span data-stu-id="dc222-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="dc222-115">Mohon berikan setidaknya 24 jam untuk menyelesaikan solusi.</span><span class="sxs-lookup"><span data-stu-id="dc222-115">Please give us at least 24 hours to complete a solution.</span></span>

<span data-ttu-id="dc222-116">**Penting**: jika sebuah situs, dokumen (Perpustakaan) atau daftar dihapus dan masih menunjukkan di hasil pencarian, pengguna akan menerima kesalahan 404 File tidak ditemukan ketika mencoba untuk mengakses.</span><span class="sxs-lookup"><span data-stu-id="dc222-116">**Important**: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an Error 404 File Not Found when trying to access.</span></span> <span data-ttu-id="dc222-117">Masalah ini harus login sebagai kasus dukungan untuk investigasi lebih lanjut.</span><span class="sxs-lookup"><span data-stu-id="dc222-117">This issue should be logged as a support case for further investigation.</span></span> 



