---
title: Konten tidak muncul di hasil pencarian SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a21e0047b41390f740f9e13d31cba32b13990151
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705664"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="f2223-102">Konten tidak muncul di hasil pencarian SharePoint</span><span class="sxs-lookup"><span data-stu-id="f2223-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="f2223-103">Ikuti langkah pemecahan masalah ini saat konten yang diharapkan tidak muncul di hasil penelusuran:</span><span class="sxs-lookup"><span data-stu-id="f2223-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="f2223-104">Periksa apakah **situs** yang berisi konten yang diharapkan diatur untuk membolehkan konten ditampilkan di hasil pencarian.</span><span class="sxs-lookup"><span data-stu-id="f2223-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="f2223-105">Ikuti langkah di [menampilkan konten di situs di hasil penelusuran](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="f2223-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="f2223-106">Periksa apakah **Daftar** atau **Perpustakaan** yang berisi konten yang diharapkan diatur untuk mengizinkan konten ditampilkan di hasil pencarian.</span><span class="sxs-lookup"><span data-stu-id="f2223-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="f2223-107">Ikuti langkah di [menampilkan konten dari daftar atau Perpustakaan di hasil penelusuran](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="f2223-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="f2223-108">Pastikan bahwa halaman, dokumen, atau tata letak halaman kustom diterbitkan sebagai **versi utama.**</span><span class="sxs-lookup"><span data-stu-id="f2223-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="f2223-109">Ikuti langkah 3 di [pencarian tidak mengembalikan semua hasil di SharePoint online](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="f2223-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="f2223-110">Verifikasi bahwa pengguna memiliki **izin** untuk melihat konten.</span><span class="sxs-lookup"><span data-stu-id="f2223-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="f2223-111">Ikuti langkah dalam [memahami tingkat izin di SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="f2223-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="f2223-112">Jika skema pencarian telah diubah dengan menambahkan properti terkelola baru, dengan mengedit properti terkelola, atau dengan menghapus properti terkelola, maka permintaan perayapan dan indeks ulang akan diperlukan.</span><span class="sxs-lookup"><span data-stu-id="f2223-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="f2223-113">**Mengindeks ulang** konten dengan mengikuti langkah [secara manual meminta perayapan dan mengindeks ulang situs, Perpustakaan, atau daftar](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="f2223-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="f2223-114">Ini mungkin memakan waktu beberapa saat, tunggu 24 jam sebelum memeriksa hasilnya lagi.</span><span class="sxs-lookup"><span data-stu-id="f2223-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="f2223-115">Untuk informasi lebih lanjut, lihat [mengaktifkan konten di situs untuk dapat ditelusuri](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="f2223-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
