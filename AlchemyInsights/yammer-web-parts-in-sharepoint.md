---
title: Komponen Web Yammer di SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5475"
- "9002494"
ms.openlocfilehash: d8b4043bb2889429a18c477505e7eca662943051
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664353"
---
# <a name="yammer-web-parts-in-sharepoint"></a><span data-ttu-id="7639a-102">Komponen Web Yammer di SharePoint</span><span class="sxs-lookup"><span data-stu-id="7639a-102">Yammer web parts in SharePoint</span></span>

<span data-ttu-id="7639a-103">Percakapan yammer dan Yammer menyoroti komponen Web untuk menyempurnakan kolaborasi pada halaman SharePoint modern dan klasik.</span><span class="sxs-lookup"><span data-stu-id="7639a-103">Yammer Conversations and Yammer Highlights web parts enhance collaboration on modern and classic SharePoint pages.</span></span> <span data-ttu-id="7639a-104">Untuk informasi selengkapnya, lihat [percakapan yammer](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#conversations)  dan  [sorotan yammer](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#highlights).</span><span class="sxs-lookup"><span data-stu-id="7639a-104">For more info, see [Yammer Conversations](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#conversations)  and  [Yammer Highlights](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#highlights).</span></span>    

<span data-ttu-id="7639a-105">Komponen Web percakapan Yammer modern diperbarui ke pengalaman Yammer yang baru dan tersedia untuk penyewa rilis bertarget.</span><span class="sxs-lookup"><span data-stu-id="7639a-105">The modern Yammer Conversations web part is being updated to the new Yammer experience and is available for Targeted Release tenants.</span></span> <span data-ttu-id="7639a-106">Peluncuran GA telah dimulai.</span><span class="sxs-lookup"><span data-stu-id="7639a-106">GA rollout has started.</span></span> <span data-ttu-id="7639a-107">Fitur baru mencakup kemampuan untuk memulai percakapan dengan postingan (pertanyaan, Polling, pujian) dan untuk menandai jawaban terbaik langsung dari SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7639a-107">New features include the ability to start a conversation with any post (Questions, Polls, Praise) and to mark best answers directly from SharePoint.</span></span> <span data-ttu-id="7639a-108">Untuk informasi selengkapnya, lihat [istilah dan tanya jawab umum pelanggan Yammer](https://docs.microsoft.com/yammer/get-started-with-yammer/newyammer-faq).</span><span class="sxs-lookup"><span data-stu-id="7639a-108">For more info, see [New Yammer customer terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/newyammer-faq).</span></span>

 <span data-ttu-id="7639a-109">Untuk memahami komponen Web dan konfigurasi yang tepat untuk Anda, lihat [menggunakan komponen Web Yammer di SharePoint online](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da).</span><span class="sxs-lookup"><span data-stu-id="7639a-109">To understand which web part and configuration is right for you, see [Use a Yammer web part in SharePoint Online](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da).</span></span>  

<span data-ttu-id="7639a-110">**Menggunakan komponen web dengan SharePoint Server**</span><span class="sxs-lookup"><span data-stu-id="7639a-110">**Using web parts with SharePoint Server**</span></span>  

<span data-ttu-id="7639a-111">Komponen Web bisa digunakan di halaman modern dan klasik dalam lingkungan di tempat.</span><span class="sxs-lookup"><span data-stu-id="7639a-111">Web parts can be used in modern and classic pages within on-premises environments.</span></span>

- <span data-ttu-id="7639a-112">Untuk informasi selengkapnya tentang halaman modern, lihat [menambahkan umpan Yammer ke halaman modern di SharePoint Server 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-modern-page-in-sharepoint-server-2019).</span><span class="sxs-lookup"><span data-stu-id="7639a-112">For more info about modern pages, see [Add a Yammer feed to a modern page in SharePoint Server 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-modern-page-in-sharepoint-server-2019).</span></span> 
- <span data-ttu-id="7639a-113">Untuk informasi selengkapnya tentang halaman klasik, lihat [menambahkan umpan Yammer ke halaman klasik di server SharePoint 2013, 2016, dan 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-classic-page-in-sharepoint-servers-2013-2016-and-2019).</span><span class="sxs-lookup"><span data-stu-id="7639a-113">For more info about classic pages, see [Add a Yammer feed to a classic page in SharePoint Servers 2013, 2016, and 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-classic-page-in-sharepoint-servers-2013-2016-and-2019).</span></span>

<span data-ttu-id="7639a-114">**Embed Yammer**</span><span class="sxs-lookup"><span data-stu-id="7639a-114">**Yammer Embed**</span></span>  

<span data-ttu-id="7639a-115">Gunakan alat konfigurasi Semat untuk menguji penggunaan Semat.</span><span class="sxs-lookup"><span data-stu-id="7639a-115">Use the Embed Configuration tool to test Embed usage.</span></span> <span data-ttu-id="7639a-116">Pembaruan mendatang untuk disematkan akan memungkinkan pengalaman Yammer yang baru.</span><span class="sxs-lookup"><span data-stu-id="7639a-116">A future update to Embed will enable the new Yammer experience.</span></span> <span data-ttu-id="7639a-117">Untuk informasi selengkapnya, lihat [alat konfigurasi embed Yammer](https://aka.ms/YammerEmbedConfigureTool).</span><span class="sxs-lookup"><span data-stu-id="7639a-117">For more info, see the [Yammer Embed Configuration tool](https://aka.ms/YammerEmbedConfigureTool).</span></span> <span data-ttu-id="7639a-118">Untuk memahami komponen embed Yammer dengan lebih baik, lihat [menyematkan umpan](https://aka.ms/YammerDevDocs).</span><span class="sxs-lookup"><span data-stu-id="7639a-118">To better understand the Yammer Embed component, see [Embed Feed](https://aka.ms/YammerDevDocs).</span></span>

<span data-ttu-id="7639a-119">**Masalah yang diketahui dan keterbatasan**</span><span class="sxs-lookup"><span data-stu-id="7639a-119">**Known issues and limitations**</span></span>

- <span data-ttu-id="7639a-120">Id grup tidak tersedia dari URL Yammer baru, yang telah berubah.</span><span class="sxs-lookup"><span data-stu-id="7639a-120">Group IDs are not available from new Yammer URLs, which have changed.</span></span> <span data-ttu-id="7639a-121">Kembali ke mode klasik untuk mendapatkan id grup atau ID lainnya dari URL.</span><span class="sxs-lookup"><span data-stu-id="7639a-121">Switch back to classic mode to obtain group IDs or other IDs from URLs.</span></span>
- <span data-ttu-id="7639a-122">Domain kustom (Vanity) tidak didukung.</span><span class="sxs-lookup"><span data-stu-id="7639a-122">Custom (vanity) domains are not supported.</span></span>
- <span data-ttu-id="7639a-123">Embed Yammer tidak dioptimalkan untuk perangkat seluler.</span><span class="sxs-lookup"><span data-stu-id="7639a-123">Yammer Embed is not optimized for mobile.</span></span> <span data-ttu-id="7639a-124">Gunakan Halaman modern dengan komponen Web percakapan Yammer untuk pengalaman terbaik.</span><span class="sxs-lookup"><span data-stu-id="7639a-124">Use modern pages with the Yammer Conversations web part for the best experience.</span></span>
- <span data-ttu-id="7639a-125">Tema kustom dapat mempengaruhi tampilan dan kegunaan komponen Web percakapan Yammer.</span><span class="sxs-lookup"><span data-stu-id="7639a-125">Custom themes can affect the appearance and usability of the Yammer Conversations web part.</span></span> <span data-ttu-id="7639a-126">Membuka kasus dukungan untuk melaporkan masalah.</span><span class="sxs-lookup"><span data-stu-id="7639a-126">Open a support case to report issues.</span></span>