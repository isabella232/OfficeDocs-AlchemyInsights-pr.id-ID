---
title: Konten tidak muncul dalam hasil pencarian SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 1/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: ffb6bf349f9e8c2323186a8fc3183325d1d7e1bf
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36517034"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="0b7d5-102">Konten tidak muncul dalam hasil pencarian SharePoint</span><span class="sxs-lookup"><span data-stu-id="0b7d5-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="0b7d5-103">Ikuti langkah pemecahan masalah ketika konten yang diharapkan tidak muncul dalam hasil pencarian:</span><span class="sxs-lookup"><span data-stu-id="0b7d5-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="0b7d5-104">Memeriksa **situs** yang berisi konten diharapkan diatur untuk memungkinkan konten yang muncul dalam hasil pencarian.</span><span class="sxs-lookup"><span data-stu-id="0b7d5-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="0b7d5-105">Ikuti langkah-langkah dalam [menunjukkan konten situs dalam hasil pencarian](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="0b7d5-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="0b7d5-106">Periksa **Daftar** atau **Perpustakaan** yang berisi konten diharapkan diatur untuk memungkinkan konten yang muncul dalam hasil pencarian.</span><span class="sxs-lookup"><span data-stu-id="0b7d5-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="0b7d5-107">Ikuti langkah-langkah di [Tampilkan isi dari daftar atau Perpustakaan dalam hasil pencarian](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="0b7d5-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="0b7d5-108">Memverifikasi bahwa halaman, dokumen, atau tata letak halaman kustom diterbitkan sebagai **versi Mayor.**</span><span class="sxs-lookup"><span data-stu-id="0b7d5-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="0b7d5-109">Ikuti langkah 3 dalam [pencarian tidak kembali semua hasil dalam SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="0b7d5-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="0b7d5-110">Pastikan bahwa pengguna memiliki **izin** untuk melihat konten.</span><span class="sxs-lookup"><span data-stu-id="0b7d5-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="0b7d5-111">Ikuti langkah-langkah dalam [pemahaman tingkat izin di SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="0b7d5-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="0b7d5-112">Jika skema Cari telah berubah dengan menambahkan properti dikelola baru, dengan mengedit properti yang dikelola atau dengan menghapus properti yang dikelola kemudian meminta merangkak dan mengindeks ulang akan diperlukan.</span><span class="sxs-lookup"><span data-stu-id="0b7d5-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="0b7d5-113">**Kembali indeks** konten dengan mengikuti langkah-langkah di [secara manual meminta merangkak dan mengindeks ulang situs, Perpustakaan atau daftar](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="0b7d5-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="0b7d5-114">Ini mungkin memakan waktu cukup lama, tunggu selama 24 jam sebelum memeriksa hasil lagi.</span><span class="sxs-lookup"><span data-stu-id="0b7d5-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="0b7d5-115">Untuk selengkapnya, lihat [mengaktifkan konten di situs harus dicari](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="0b7d5-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
