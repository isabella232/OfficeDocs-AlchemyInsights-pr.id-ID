---
title: Mengelola skema pencarian di SharePoint online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f2d8d3e07fe32d21af484e4c59e0f5ac6fe8081c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770554"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="f0d32-102">Mengelola skema pencarian di SharePoint online</span><span class="sxs-lookup"><span data-stu-id="f0d32-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="f0d32-103">Skema pencarian mengontrol apa yang bisa dicari pengguna, bagaimana pengguna bisa mencari, dan bagaimana Anda bisa menyajikan hasil di situs web pencarian Anda.</span><span class="sxs-lookup"><span data-stu-id="f0d32-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="f0d32-104">Lihat [mengelola skema pencarian di SharePoint online](https://docs.microsoft.com/sharepoint/manage-search-schema) untuk mempelajari cara:</span><span class="sxs-lookup"><span data-stu-id="f0d32-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="f0d32-105">Mengubah skema pencarian.</span><span class="sxs-lookup"><span data-stu-id="f0d32-105">Change the search schema.</span></span>
- <span data-ttu-id="f0d32-106">Membuat properti terkelola.</span><span class="sxs-lookup"><span data-stu-id="f0d32-106">Create managed properties.</span></span>
- <span data-ttu-id="f0d32-107">Memetakan properti rayapan peta ke properti yang dikelola.</span><span class="sxs-lookup"><span data-stu-id="f0d32-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="f0d32-108">Perhatikan hal berikut ini terkait dengan pengelolaan skema pencarian Anda:</span><span class="sxs-lookup"><span data-stu-id="f0d32-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="f0d32-109">Jika Anda menerima peringatan yang menyatakan **aplikasi dijeda** ketika membuat skema berubah, ini hanya sementara karena ada pemeliharaan layanan yang terjadi.</span><span class="sxs-lookup"><span data-stu-id="f0d32-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="f0d32-110">Jika lebih dari 24 jam telah berlalu dan Anda masih mengalami peringatan tersebut, silakan log kasus dukungan.</span><span class="sxs-lookup"><span data-stu-id="f0d32-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="f0d32-111">Saat Anda mengubah properti terkelola atau menambahkan yang baru, perubahan tersebut akan diterapkan hanya setelah konten dirayapi ulang.</span><span class="sxs-lookup"><span data-stu-id="f0d32-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="f0d32-112">Di SharePoint online, Crawling terjadi secara otomatis berdasarkan jadwal perayapan yang ditentukan.</span><span class="sxs-lookup"><span data-stu-id="f0d32-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="f0d32-113">Untuk memastikan bahwa perubahan Anda dirayapi, Anda bisa secara khusus [meminta pengindeksan ulang daftar atau pustaka](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span><span class="sxs-lookup"><span data-stu-id="f0d32-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="f0d32-114">Untuk gambaran umum lengkap tentang skema pencarian, lihat [memperkenalkan skema pencarian](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="f0d32-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


