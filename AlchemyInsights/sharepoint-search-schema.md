---
title: Mengelola skema pencarian di SharePoint online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 9836cf139e97fc556995a8f0ad38c51c5c2392ac
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/15/2019
ms.locfileid: "40042966"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="2312c-102">Mengelola skema pencarian di SharePoint online</span><span class="sxs-lookup"><span data-stu-id="2312c-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="2312c-103">Skema pencarian mengontrol apa yang dapat dicari pengguna, bagaimana pengguna dapat mencari, dan bagaimana Anda dapat mempresentasikan hasilnya di situs web pencarian Anda.</span><span class="sxs-lookup"><span data-stu-id="2312c-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="2312c-104">Lihat [mengelola skema pencarian di SharePoint online](https://docs.microsoft.com/sharepoint/manage-search-schema) untuk mempelajari cara:</span><span class="sxs-lookup"><span data-stu-id="2312c-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="2312c-105">Mengubah skema pencarian.</span><span class="sxs-lookup"><span data-stu-id="2312c-105">Change the search schema.</span></span>
- <span data-ttu-id="2312c-106">Buat properti terkelola.</span><span class="sxs-lookup"><span data-stu-id="2312c-106">Create managed properties.</span></span>
- <span data-ttu-id="2312c-107">Peta meng-Crawl peta yang dirayapi properti ke properti terkelola.</span><span class="sxs-lookup"><span data-stu-id="2312c-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="2312c-108">Catatan berikut ini dalam hal mengelola skema pencarian Anda:</span><span class="sxs-lookup"><span data-stu-id="2312c-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="2312c-109">Jika Anda menerima peringatan yang menyatakan **aplikasi dijeda** saat membuat skema perubahan, ini hanya sementara karena ada pemeliharaan layanan yang terjadi.</span><span class="sxs-lookup"><span data-stu-id="2312c-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="2312c-110">Jika lebih dari 24 jam telah berlalu dan Anda masih mengalami peringatan, silakan log kasus dukungan.</span><span class="sxs-lookup"><span data-stu-id="2312c-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="2312c-111">Bila Anda mengubah properti terkelola atau menambahkan yang baru, perubahan akan diterapkan hanya setelah konten telah dirayapi ulang.</span><span class="sxs-lookup"><span data-stu-id="2312c-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="2312c-112">Di SharePoint online, perayapan terjadi secara otomatis berdasarkan jadwal perayapan yang ditetapkan.</span><span class="sxs-lookup"><span data-stu-id="2312c-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="2312c-113">Untuk memastikan bahwa perubahan Anda dirayapi, Anda dapat secara khusus [meminta pengindeksan ulang daftar atau Perpustakaan](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span><span class="sxs-lookup"><span data-stu-id="2312c-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="2312c-114">Untuk ringkasan lengkap tentang skema pencarian, lihat [memperkenalkan skema pencarian](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="2312c-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


