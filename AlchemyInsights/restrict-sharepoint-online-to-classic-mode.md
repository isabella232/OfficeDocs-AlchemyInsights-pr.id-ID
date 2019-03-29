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
ms.openlocfilehash: c51e48fe5694f964aef74c2973f774b44415ebb8
ms.sourcegitcommit: 21cfb213183188d32a3743f66db10a8463019965
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/28/2019
ms.locfileid: "30955995"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="521ef-102">Membatasi SharePoint Online ke modus klasik</span><span class="sxs-lookup"><span data-stu-id="521ef-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="521ef-103">Beberapa organisasi masih memerlukan pengalaman modus klasik.</span><span class="sxs-lookup"><span data-stu-id="521ef-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="521ef-104">Sementara ada tidak ada rencana untuk menghapus modus klasik pada tingkat yang rinci, mulai April 1,2019, itu tidak akan mungkin untuk membatasi seluruh organisasi (penyewa) untuk modus klasik untuk daftar dan perpustakaan.</span><span class="sxs-lookup"><span data-stu-id="521ef-104">While there are no plans to remove classic mode at a granular level, starting April 1,2019, it will no longer be possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="521ef-105">Admin akan memiliki pilihan berikut untuk mengelola daftar individu dan perpustakaan dalam modus klasik yang menggunakan butiran switch keluar yang kami sediakan di tingkat berikut:</span><span class="sxs-lookup"><span data-stu-id="521ef-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="521ef-106">situs koleksi</span><span class="sxs-lookup"><span data-stu-id="521ef-106">site collection</span></span>
- <span data-ttu-id="521ef-107">situs</span><span class="sxs-lookup"><span data-stu-id="521ef-107">site</span></span>
- <span data-ttu-id="521ef-108">Daftar</span><span class="sxs-lookup"><span data-stu-id="521ef-108">list</span></span>
- <span data-ttu-id="521ef-109">Perpustakaan</span><span class="sxs-lookup"><span data-stu-id="521ef-109">library</span></span>

<span data-ttu-id="521ef-110">Selain itu, daftar yang menggunakan fitur tertentu dan kustomisasi yang tidak didukung oleh modern akan masih akan secara otomatis beralih ke modus klasik.</span><span class="sxs-lookup"><span data-stu-id="521ef-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="521ef-111">Setelah April 1, daftar dan perpustakaan yang berada dalam modus klasik sebagai hasil dari penyewa keluar akan secara otomatis dikelola di tingkat situs dan daftar tingkat.</span><span class="sxs-lookup"><span data-stu-id="521ef-111">After April 1, lists and libraries that are in classic mode as a result of tenant opt-out will automatically be managed at the site level and list level.</span></span>

<span data-ttu-id="521ef-112">Jika Anda memerlukan modus klasik Lihat informasi lebih lanjut di sini dan PnP Powershell instruksi berikut yang menggambarkan pilihan dan peralatan Anda dapat menggunakan hari ini untuk mempersiapkan penghapusan penyewa tingkat keluar pada April 1.</span><span class="sxs-lookup"><span data-stu-id="521ef-112">If you require classic mode please see more information here and PnP Powershell instruction here that describes options and tools you can use today to prepare for the removal of the tenant level opt-out on April 1.</span></span>
