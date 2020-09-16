---
title: Membatasi mode SharePoint online ke klasik
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 1887bf64df98bf90a1902250633d5774178dfa2f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751425"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="dfdcf-102">Membatasi mode SharePoint online ke klasik</span><span class="sxs-lookup"><span data-stu-id="dfdcf-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="dfdcf-103">Beberapa organisasi masih memerlukan pengalaman mode klasik.</span><span class="sxs-lookup"><span data-stu-id="dfdcf-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="dfdcf-104">Meskipun tidak ada rencana untuk menghapus mode klasik pada tingkat granular, tidak mungkin lagi membatasi seluruh organisasi (penyewa) ke mode klasik untuk daftar dan pustaka.</span><span class="sxs-lookup"><span data-stu-id="dfdcf-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="dfdcf-105">Admin akan memiliki opsi berikut ini untuk mengelola daftar dan pustaka individual dalam mode klasik menggunakan Sakelar tidak ikut granular yang kami sediakan pada tingkatan berikut ini:</span><span class="sxs-lookup"><span data-stu-id="dfdcf-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="dfdcf-106">kumpulan situs</span><span class="sxs-lookup"><span data-stu-id="dfdcf-106">site collection</span></span>
- <span data-ttu-id="dfdcf-107">site</span><span class="sxs-lookup"><span data-stu-id="dfdcf-107">site</span></span>
- <span data-ttu-id="dfdcf-108">List</span><span class="sxs-lookup"><span data-stu-id="dfdcf-108">list</span></span>
- <span data-ttu-id="dfdcf-109">Koleksi</span><span class="sxs-lookup"><span data-stu-id="dfdcf-109">library</span></span>

<span data-ttu-id="dfdcf-110">Selain itu, daftar yang menggunakan fitur dan kustomisasi tertentu yang tidak didukung oleh modern masih akan dialihkan secara otomatis ke mode klasik.</span><span class="sxs-lookup"><span data-stu-id="dfdcf-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="dfdcf-111">Mulai 1 April 2019, proses untuk menonaktifkan tingkat penyewa tidak memilih daftar dan pustaka modern akan dimulai dan berlanjut hingga 31 Mei 2019.</span><span class="sxs-lookup"><span data-stu-id="dfdcf-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="dfdcf-112">Daftar dan pustaka yang berada dalam mode klasik sebagai hasil dari penyisihan penyewa akan bergeser ke modern secara otomatis.</span><span class="sxs-lookup"><span data-stu-id="dfdcf-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="dfdcf-113">Jika Anda memerlukan mode klasik silakan lihat informasi selengkapnya [di sini](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) dan instruksi PowerShell PNP [di sini](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) yang menguraikan opsi dan alat yang bisa Anda gunakan hari ini untuk menggunakan pengalaman mode klasik.</span><span class="sxs-lookup"><span data-stu-id="dfdcf-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
