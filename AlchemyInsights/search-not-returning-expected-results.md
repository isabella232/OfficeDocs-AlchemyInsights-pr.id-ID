---
title: 1491-pencarian-tidak-kembali-diharapkan-hasil
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 57421d459ef03049d6f931db659a5f9b253f5002
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510575"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="163ee-102">Pencarian konten tidak mengembalikan hasil yang diharapkan</span><span class="sxs-lookup"><span data-stu-id="163ee-102">Content Search not returning expected results</span></span>

<span data-ttu-id="163ee-103">Saat menjalankan pencarian konten dari Microsoft 365 keamanan & kepatuhan pusat, Anda mungkin menerima hasil pencarian tak terduga.</span><span class="sxs-lookup"><span data-stu-id="163ee-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="163ee-104">Pertimbangkan hal berikut yang dapat memengaruhi hasil penelusuran Anda:</span><span class="sxs-lookup"><span data-stu-id="163ee-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="163ee-105">**Lokasi konten dan kondisi penelusuran**: Pastikan Anda telah memilih lokasi konten yang tepat dan kondisi penelusuran.</span><span class="sxs-lookup"><span data-stu-id="163ee-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="163ee-106">Jika Anda menjalankan pencarian besar (dengan banyak lokasi), pertimbangkan untuk membelah ke dalam beberapa pencarian.</span><span class="sxs-lookup"><span data-stu-id="163ee-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="163ee-107">**Item yang diindeks sebagian**: [item yang diindeks sebagian](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) dari kotak pesan disertakan dalam perkiraan hasil penelusuran.</span><span class="sxs-lookup"><span data-stu-id="163ee-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="163ee-108">Namun, sebagian diindeks item dari situs di SharePoint dan OneDrive tidak termasuk dalam perkiraan pencarian.</span><span class="sxs-lookup"><span data-stu-id="163ee-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="163ee-109">**Pencarian kegagalan**: ketika mencari sejumlah besar kotak pesan (lebih dari 100.000 kotak surat), Anda mungkin mendapatkan galat pencarian, dengan kode GALAT seperti CS008-009 dan CS012-002).</span><span class="sxs-lookup"><span data-stu-id="163ee-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="163ee-110">Dalam kasus ini, coba lagi pencarian hanya untuk lokasi konten yang gagal.</span><span class="sxs-lookup"><span data-stu-id="163ee-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="163ee-111">Lihat [artikel ini](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) untuk informasi lebih lanjut.</span><span class="sxs-lookup"><span data-stu-id="163ee-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
