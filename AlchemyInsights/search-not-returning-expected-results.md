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
ms.custom: 1491
ms.assetid: ''
ms.openlocfilehash: 517d9b75fc3aef09c0c2d5870aa695cc0ab10f06
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/23/2019
ms.locfileid: "32383838"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="f0b24-102">Cari konten tidak kembali hasil yang diharapkan</span><span class="sxs-lookup"><span data-stu-id="f0b24-102">Content Search not returning expected results</span></span>

<span data-ttu-id="f0b24-103">Ketika menjalankan pencarian konten dari Office 365 keamanan & Compliance Center, Anda mungkin menerima hasil pencarian tak terduga.</span><span class="sxs-lookup"><span data-stu-id="f0b24-103">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="f0b24-104">Pertimbangkan hal berikut yang dapat mempengaruhi hasil pencarian Anda:</span><span class="sxs-lookup"><span data-stu-id="f0b24-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="f0b24-105">**Lokasi konten dan kondisi pencarian**: Pastikan Anda telah memilih lokasi konten yang tepat dan Cari kondisi.</span><span class="sxs-lookup"><span data-stu-id="f0b24-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="f0b24-106">Jika Anda menjalankan pencarian besar (dengan banyak lokasi), pertimbangkan untuk membagi menjadi beberapa pencarian.</span><span class="sxs-lookup"><span data-stu-id="f0b24-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="f0b24-107">**Sebagian diindeks item**: [sebagian diindeks item](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) dari kotak pesan disertakan dalam hasil pencarian yang diperkirakan.</span><span class="sxs-lookup"><span data-stu-id="f0b24-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="f0b24-108">Namun, sebagian diindeks item dari situs di SharePoint dan OneDrive tidak termasuk dalam perkiraan Cari.</span><span class="sxs-lookup"><span data-stu-id="f0b24-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="f0b24-109">**Cari kegagalan**: ketika mencari sejumlah besar kotak pesan (kotak pesan lebih dari 100.000), Anda mungkin mendapatkan Cari kesalahan, dengan kode kesalahan seperti CS008-009 dan CS012-002).</span><span class="sxs-lookup"><span data-stu-id="f0b24-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="f0b24-110">Dalam kasus ini, coba lagi hanya mencari lokasi konten yang gagal.</span><span class="sxs-lookup"><span data-stu-id="f0b24-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="f0b24-111">Lihat [artikel ini](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) untuk informasi lebih lanjut.</span><span class="sxs-lookup"><span data-stu-id="f0b24-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
