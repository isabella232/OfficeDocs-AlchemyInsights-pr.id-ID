---
title: Membatasi SharePoint Online ke modus klasik
ms.author: kirks
author: Techwriter40
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.openlocfilehash: 76f0b5ed67d3220559d25dfd72c7535181a4513b
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/07/2019
ms.locfileid: "34761762"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="f1c71-102">Membatasi SharePoint Online ke modus klasik</span><span class="sxs-lookup"><span data-stu-id="f1c71-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="f1c71-103">Beberapa organisasi masih memerlukan pengalaman modus klasik.</span><span class="sxs-lookup"><span data-stu-id="f1c71-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="f1c71-104">Sementara ada tidak ada rencana untuk menghapus modus klasik pada tingkat yang rinci, hal ini tidak mungkin lagi untuk membatasi seluruh organisasi (penyewa) ke modus klasik untuk daftar dan perpustakaan.</span><span class="sxs-lookup"><span data-stu-id="f1c71-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="f1c71-105">Admin akan memiliki pilihan berikut untuk mengelola daftar individu dan perpustakaan dalam modus klasik yang menggunakan butiran switch keluar yang kami sediakan di tingkat berikut:</span><span class="sxs-lookup"><span data-stu-id="f1c71-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="f1c71-106">situs koleksi</span><span class="sxs-lookup"><span data-stu-id="f1c71-106">site collection</span></span>
- <span data-ttu-id="f1c71-107">situs</span><span class="sxs-lookup"><span data-stu-id="f1c71-107">site</span></span>
- <span data-ttu-id="f1c71-108">Daftar</span><span class="sxs-lookup"><span data-stu-id="f1c71-108">list</span></span>
- <span data-ttu-id="f1c71-109">Perpustakaan</span><span class="sxs-lookup"><span data-stu-id="f1c71-109">library</span></span>

<span data-ttu-id="f1c71-110">Selain itu, daftar yang menggunakan fitur tertentu dan kustomisasi yang tidak didukung oleh modern akan masih akan secara otomatis beralih ke modus klasik.</span><span class="sxs-lookup"><span data-stu-id="f1c71-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="f1c71-111">Mulai 1 April 2019, proses untuk menonaktifkan tingkat penyewa menyisih dari daftar modern dan Perpustakaan akan mulai dan terus melalui 31 Mei 2019.</span><span class="sxs-lookup"><span data-stu-id="f1c71-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="f1c71-112">Daftar dan perpustakaan yang berada dalam modus klasik sebagai hasil dari penyewa keluar akan secara otomatis beralih ke modern.</span><span class="sxs-lookup"><span data-stu-id="f1c71-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="f1c71-113">Jika Anda memerlukan modus klasik Lihat informasi lebih lanjut [di sini](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) dan instruksi PnP Powershell [di sini](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) yang menggambarkan pilihan dan alat-alat yang dapat Anda gunakan hari menggunakan pengalaman modus klasik.</span><span class="sxs-lookup"><span data-stu-id="f1c71-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
