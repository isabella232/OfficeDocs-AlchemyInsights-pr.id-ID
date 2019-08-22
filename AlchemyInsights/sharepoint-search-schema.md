---
title: Mengelola skema Cari SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 704fb3b682d23220d61192e383d7d80f59f27933
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36502810"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="bf3b9-102">Mengelola skema Cari SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="bf3b9-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="bf3b9-103">Cari skema kontrol apa pengguna dapat mencari, bagaimana pengguna dapat mencari itu, dan bagaimana Anda dapat menampilkan hasil pencarian situs Anda.</span><span class="sxs-lookup"><span data-stu-id="bf3b9-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="bf3b9-104">Lihat [mengelola skema Cari di SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) untuk belajar bagaimana untuk:</span><span class="sxs-lookup"><span data-stu-id="bf3b9-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="bf3b9-105">Mengubah skema Cari.</span><span class="sxs-lookup"><span data-stu-id="bf3b9-105">Change the search schema.</span></span>
- <span data-ttu-id="bf3b9-106">Membuat properti yang dikelola.</span><span class="sxs-lookup"><span data-stu-id="bf3b9-106">Create managed properties.</span></span>
- <span data-ttu-id="bf3b9-107">Peta merangkak peta merangkak properti properti yang dikelola.</span><span class="sxs-lookup"><span data-stu-id="bf3b9-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="bf3b9-108">Perhatikan hal berikut dalam hal untuk mengelola skema Cari:</span><span class="sxs-lookup"><span data-stu-id="bf3b9-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="bf3b9-109">Jika Anda menerima peringatan menyatakan **aplikasi berhenti** ketika membuat perubahan skema, hal ini hanya sementara sebagai ada jasa maintenance terjadi.</span><span class="sxs-lookup"><span data-stu-id="bf3b9-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="bf3b9-110">Jika lebih dari 24 jam telah berlalu dan Anda masih mengalami peringatan, silahkan log kasus dukungan.</span><span class="sxs-lookup"><span data-stu-id="bf3b9-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="bf3b9-111">Bila Anda mengubah properti yang dikelola atau menambahkan yang baru, perubahan akan berlaku hanya setelah konten telah kembali merangkak.</span><span class="sxs-lookup"><span data-stu-id="bf3b9-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="bf3b9-112">Dalam SharePoint Online, merangkak terjadi secara otomatis berdasarkan jadwal didefinisikan merangkak.</span><span class="sxs-lookup"><span data-stu-id="bf3b9-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="bf3b9-113">Untuk memastikan bahwa perubahan Anda merangkak, Anda dapat secara khusus [permintaan mengindeks ulang daftar atau Perpustakaan](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span><span class="sxs-lookup"><span data-stu-id="bf3b9-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="bf3b9-114">Untuk gambaran lengkap dari skema Cari, lihat [Memperkenalkan Cari skema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="bf3b9-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


