---
title: Konten tidak muncul di hasil pencarian SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a57711434d653f5d5667776916c9251bba2370e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713133"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="d84f7-102">Konten tidak muncul di hasil pencarian SharePoint</span><span class="sxs-lookup"><span data-stu-id="d84f7-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="d84f7-103">Ikuti langkah pemecahan masalah ini jika konten yang diharapkan tidak muncul di hasil pencarian:</span><span class="sxs-lookup"><span data-stu-id="d84f7-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="d84f7-104">Periksa bahwa **situs** yang berisi konten yang diharapkan diatur untuk memperbolehkan konten muncul di hasil pencarian.</span><span class="sxs-lookup"><span data-stu-id="d84f7-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="d84f7-105">Ikuti langkah-langkah dalam [memperlihatkan konten di situs dalam hasil pencarian](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="d84f7-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="d84f7-106">Periksa bahwa **Daftar** atau **pustaka** yang berisi konten yang diharapkan diatur untuk memperbolehkan konten muncul di hasil pencarian.</span><span class="sxs-lookup"><span data-stu-id="d84f7-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="d84f7-107">Ikuti langkah-langkah dalam [memperlihatkan konten dari daftar atau pustaka dalam hasil pencarian](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="d84f7-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="d84f7-108">Verifikasi bahwa tata letak halaman, dokumen, atau halaman kustom diterbitkan sebagai **versi utama.**</span><span class="sxs-lookup"><span data-stu-id="d84f7-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="d84f7-109">Ikuti langkah 3 di [pencarian tidak mengembalikan semua hasil di SharePoint online](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="d84f7-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="d84f7-110">Verifikasi bahwa pengguna memiliki **izin** untuk menampilkan konten.</span><span class="sxs-lookup"><span data-stu-id="d84f7-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="d84f7-111">Ikuti langkah-langkah dalam [memahami tingkat izin di SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="d84f7-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="d84f7-112">Jika skema pencarian telah diubah dengan menambahkan properti yang dikelola baru, dengan mengedit properti yang dikelola, atau dengan menghapus properti yang dikelola, maka meminta Crawl dan mengindeks ulang akan diperlukan.</span><span class="sxs-lookup"><span data-stu-id="d84f7-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="d84f7-113">**Mengindeks ulang** konten dengan mengikuti langkah-langkah dalam [permintaan secara manual merayapi dan mengindeks ulang situs, pustaka atau daftar](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="d84f7-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="d84f7-114">Ini mungkin memakan waktu beberapa saat, tunggu 24 jam sebelum memeriksa hasilnya lagi.</span><span class="sxs-lookup"><span data-stu-id="d84f7-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="d84f7-115">Untuk informasi selengkapnya, lihat [mengaktifkan konten di situs yang akan dicari](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="d84f7-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
