---
title: 1490-pemecahan masalah-eDiscovery-kegagalan
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
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277829"
---
# <a name="troubleshoot-content-search-errors"></a><span data-ttu-id="3ac7a-102">Memecahkan masalah kesalahan pencarian konten</span><span class="sxs-lookup"><span data-stu-id="3ac7a-102">Troubleshoot Content Search errors</span></span>

<span data-ttu-id="3ac7a-103">Apakah Anda mengalami masalah dengan pencarian konten atau mendapatkan kegagalan ketika mengekspor hasil pencarian?</span><span class="sxs-lookup"><span data-stu-id="3ac7a-103">Are you experiencing problems with Content Search or getting failures when you export search results?</span></span>

<span data-ttu-id="3ac7a-104">Misalnya, Apakah Anda menerima hal berikut ini saat menjalankan pencarian?</span><span class="sxs-lookup"><span data-stu-id="3ac7a-104">For example, are you receiving the following when running searches?</span></span>

- <span data-ttu-id="3ac7a-105">Kesalahan CS008 atau CS012</span><span class="sxs-lookup"><span data-stu-id="3ac7a-105">CS008 or CS012 errors</span></span>

- <span data-ttu-id="3ac7a-106">Kesalahan sibuk/waktu habis server</span><span class="sxs-lookup"><span data-stu-id="3ac7a-106">Server busy/timeout errors</span></span>

- <span data-ttu-id="3ac7a-107">Terjadi galat aplikasi</span><span class="sxs-lookup"><span data-stu-id="3ac7a-107">Application error occurred</span></span>

<span data-ttu-id="3ac7a-108">Atau saat mencari atau mengekspor hasil dari sejumlah besar kotak surat (lebih dari 100.000 kotak surat), Apakah Anda mendapatkan kesalahan ekspor?</span><span class="sxs-lookup"><span data-stu-id="3ac7a-108">Or when searching or exporting results from a large number of mailboxes (over 100,000 mailboxes), are you getting export errors?</span></span>

<span data-ttu-id="3ac7a-109">Untuk tipe kesalahan ini, coba Cari lokasi konten yang gagal.</span><span class="sxs-lookup"><span data-stu-id="3ac7a-109">For these types of errors, retry the search for the content locations that have failed.</span></span> <span data-ttu-id="3ac7a-110">Lihat  [artikel ini](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) untuk informasi selengkapnya.</span><span class="sxs-lookup"><span data-stu-id="3ac7a-110">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>

<span data-ttu-id="3ac7a-111">Jika Anda mengekspor lebih dari 100K kotak surat, Anda perlu menggunakan PowerShell berikut untuk mengunduh hasil ekspor:  [mengekspor hasil dari kotak surat lebih dari 100k](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="3ac7a-111">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>
