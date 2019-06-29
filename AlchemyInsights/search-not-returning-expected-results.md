---
title: 1491-Search-not-Returning-Expected-Results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d25c1ef2e0e746432472a436cb11d25b5db5596c
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/28/2019
ms.locfileid: "35355880"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="e7f1b-102">Cari konten tidak kembali hasil yang diharapkan</span><span class="sxs-lookup"><span data-stu-id="e7f1b-102">Content Search not returning expected results</span></span>

<span data-ttu-id="e7f1b-103">Ketika menjalankan pencarian konten dari Office 365 keamanan & Compliance Center, Anda mungkin menerima hasil pencarian tak terduga.</span><span class="sxs-lookup"><span data-stu-id="e7f1b-103">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="e7f1b-104">Pertimbangkan hal berikut yang dapat mempengaruhi hasil pencarian Anda:</span><span class="sxs-lookup"><span data-stu-id="e7f1b-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="e7f1b-105">**Lokasi konten dan kondisi pencarian**: Pastikan Anda telah memilih lokasi konten yang tepat dan Cari kondisi.</span><span class="sxs-lookup"><span data-stu-id="e7f1b-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="e7f1b-106">Jika Anda menjalankan pencarian besar (dengan banyak lokasi), pertimbangkan untuk membagi menjadi beberapa pencarian.</span><span class="sxs-lookup"><span data-stu-id="e7f1b-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="e7f1b-107">**Sebagian diindeks item**: [sebagian diindeks item](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) dari kotak pesan disertakan dalam hasil pencarian yang diperkirakan.</span><span class="sxs-lookup"><span data-stu-id="e7f1b-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="e7f1b-108">Namun, sebagian diindeks item dari situs di SharePoint dan OneDrive tidak termasuk dalam perkiraan Cari.</span><span class="sxs-lookup"><span data-stu-id="e7f1b-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="e7f1b-109">**Cari kegagalan**: ketika mencari sejumlah besar kotak pesan (kotak pesan lebih dari 100.000), Anda mungkin mendapatkan Cari kesalahan, dengan kode kesalahan seperti CS008-009 dan CS012-002).</span><span class="sxs-lookup"><span data-stu-id="e7f1b-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="e7f1b-110">Dalam kasus ini, coba lagi hanya mencari lokasi konten yang gagal.</span><span class="sxs-lookup"><span data-stu-id="e7f1b-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="e7f1b-111">Lihat [artikel ini](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) untuk informasi lebih lanjut.</span><span class="sxs-lookup"><span data-stu-id="e7f1b-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
