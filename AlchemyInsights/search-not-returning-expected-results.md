---
title: 1491-pencarian-tidak dikembalikan-diharapkan-hasil
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740477"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="41878-102">Pencarian konten tidak mengembalikan hasil yang diharapkan</span><span class="sxs-lookup"><span data-stu-id="41878-102">Content Search not returning expected results</span></span>

<span data-ttu-id="41878-103">Saat menjalankan pencarian konten dari pusat kepatuhan & keamanan Microsoft 365, Anda mungkin menerima hasil pencarian yang tidak diharapkan.</span><span class="sxs-lookup"><span data-stu-id="41878-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="41878-104">Pertimbangkan hal-hal berikut yang bisa mempengaruhi hasil pencarian Anda:</span><span class="sxs-lookup"><span data-stu-id="41878-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="41878-105">**Lokasi konten dan kondisi pencarian**: Pastikan Anda telah memilih lokasi konten dan kondisi pencarian yang tepat.</span><span class="sxs-lookup"><span data-stu-id="41878-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="41878-106">Jika Anda menjalankan pencarian besar (dengan banyak lokasi), pertimbangkan untuk memisahkan dalam beberapa pencarian.</span><span class="sxs-lookup"><span data-stu-id="41878-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="41878-107">**Item yang diindeks sebagian**:  [item yang diindeks sebagian](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) dari kotak surat disertakan dalam hasil pencarian yang diperkirakan.</span><span class="sxs-lookup"><span data-stu-id="41878-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="41878-108">Namun, sebagian item yang diindeks dari situs di SharePoint dan OneDrive tidak disertakan dalam perkiraan pencarian.</span><span class="sxs-lookup"><span data-stu-id="41878-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="41878-109">**Kegagalan pencarian**: saat mencari sejumlah besar kotak surat (lebih dari 100.000 kotak surat), Anda mungkin mendapatkan kesalahan pencarian, dengan kode kesalahan seperti CS008-009 dan CS012-002).</span><span class="sxs-lookup"><span data-stu-id="41878-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="41878-110">Dalam kasus ini, coba lagi pencarian untuk lokasi konten gagal.</span><span class="sxs-lookup"><span data-stu-id="41878-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="41878-111">Lihat  [artikel ini](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) untuk informasi selengkapnya.</span><span class="sxs-lookup"><span data-stu-id="41878-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
