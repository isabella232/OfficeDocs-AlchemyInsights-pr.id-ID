---
title: Membatasi SharePoint online untuk mode klasik
ms.author: pebaum
author: pebaum
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: b58a1c3fc331c739080542917d8945c090ec0d94
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048763"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="b7884-102">Membatasi SharePoint online untuk mode klasik</span><span class="sxs-lookup"><span data-stu-id="b7884-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="b7884-103">Beberapa organisasi masih memerlukan pengalaman mode klasik.</span><span class="sxs-lookup"><span data-stu-id="b7884-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="b7884-104">Meskipun tidak ada rencana untuk menghapus modus klasik pada tingkat granular, tidak mungkin lagi untuk membatasi seluruh organisasi (penyewa) ke mode klasik untuk daftar dan perpustakaan.</span><span class="sxs-lookup"><span data-stu-id="b7884-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="b7884-105">Admin akan memiliki pilihan berikut untuk mengelola masing-masing daftar dan pustaka dalam mode klasik menggunakan switch opt-out granular yang kami sediakan pada tingkat berikut:</span><span class="sxs-lookup"><span data-stu-id="b7884-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="b7884-106">koleksi situs</span><span class="sxs-lookup"><span data-stu-id="b7884-106">site collection</span></span>
- <span data-ttu-id="b7884-107">Situs</span><span class="sxs-lookup"><span data-stu-id="b7884-107">site</span></span>
- <span data-ttu-id="b7884-108">Daftar</span><span class="sxs-lookup"><span data-stu-id="b7884-108">list</span></span>
- <span data-ttu-id="b7884-109">Perpustakaan</span><span class="sxs-lookup"><span data-stu-id="b7884-109">library</span></span>

<span data-ttu-id="b7884-110">Selain itu, daftar yang menggunakan fitur tertentu dan kustomisasi yang tidak didukung oleh modern masih akan secara otomatis beralih ke mode klasik.</span><span class="sxs-lookup"><span data-stu-id="b7884-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="b7884-111">Mulai April 1, 2019, proses untuk menonaktifkan tingkat penyewa memilih keluar dari daftar modern dan Perpustakaan akan mulai dan terus melalui 31 Mei 2019.</span><span class="sxs-lookup"><span data-stu-id="b7884-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="b7884-112">Daftar dan perpustakaan yang dalam mode klasik sebagai hasil dari penyewa opt-out secara otomatis akan bergeser ke modern.</span><span class="sxs-lookup"><span data-stu-id="b7884-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="b7884-113">Jika Anda memerlukan mode klasik, silakan lihat informasi lebih lanjut [di sini](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) dan instruksi PNP PowerShell [di sini](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) yang menjelaskan opsi dan alat yang dapat Anda gunakan saat ini untuk menggunakan pengalaman mode klasik.</span><span class="sxs-lookup"><span data-stu-id="b7884-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
