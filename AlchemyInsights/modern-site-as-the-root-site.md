---
title: Situs modern sebagai situs akar
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1874"
- "9000265"
ms.openlocfilehash: b30fc3258bb76c0ab4bf10af0ec9317417f7c663
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/07/2019
ms.locfileid: "36232718"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="a69d4-102">Situs modern sebagai situs akar</span><span class="sxs-lookup"><span data-stu-id="a69d4-102">Modern site as root site</span></span>

<span data-ttu-id="a69d4-103">Kami telah mulai untuk peluncuran fitur baru yang akan memungkinkan Anda untuk menukar situs akar klasik situs Anda dengan situs modern.</span><span class="sxs-lookup"><span data-stu-id="a69d4-103">We have begun to rollout a new feature that will allow you to swap your classic site root site with a modern site.</span></span> <span data-ttu-id="a69d4-104">Gunakan [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) untuk menukar lokasi situs dengan situs lain sementara pengarsipan situs asli.</span><span class="sxs-lookup"><span data-stu-id="a69d4-104">Use [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="a69d4-105">Tersedia untuk tim situs (tidak terhubung ke grup) dan komunikasi situs.</span><span class="sxs-lookup"><span data-stu-id="a69d4-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

>[!Important]
> <span data-ttu-id="a69d4-106">Tidak menghapus situs akar klasik untuk membuat situs komunikasi modern.</span><span class="sxs-lookup"><span data-stu-id="a69d4-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="a69d4-107">Hal ini tidak didukung oleh Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a69d4-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="a69d4-108">Menghapus situs akar akan membuat semua situs SharePoint dalam organisasi Anda tidak dapat diakses untuk semua pengguna, sampai Anda mengembalikan situs atau membuat situs baru di URL yang sama.</span><span class="sxs-lookup"><span data-stu-id="a69d4-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="a69d4-109">Kita akan berkomunikasi melalui pusat pesan fitur ini.</span><span class="sxs-lookup"><span data-stu-id="a69d4-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="a69d4-110">Anda harus mengharapkan fitur harus diaktifkan di penyewa Anda segera.</span><span class="sxs-lookup"><span data-stu-id="a69d4-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="a69d4-111">Masalah yang dikenal dengan menukar situs</span><span class="sxs-lookup"><span data-stu-id="a69d4-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="a69d4-112">Situs target mungkin kembali "tidak ditemukan" kesalahan (HTTP 404) untuk periode waktu yang singkat.</span><span class="sxs-lookup"><span data-stu-id="a69d4-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="a69d4-113">Konten akan perlu recrawled untuk memperbarui indeks pencarian.</span><span class="sxs-lookup"><span data-stu-id="a69d4-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="a69d4-114">Tidak ada langkah manual yang diperlukan di sini, ini akan dilakukan secara otomatis.</span><span class="sxs-lookup"><span data-stu-id="a69d4-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="a69d4-115">Apa pun yang bergantung pada "statis" link (seperti File Sync dan OneNote file) akan perlu diperbaiki secara manual.</span><span class="sxs-lookup"><span data-stu-id="a69d4-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="a69d4-116">Lokasi Server proyek mungkin perlu divalidasi untuk memastikan bahwa mereka masih berhubungan dengan benar.</span><span class="sxs-lookup"><span data-stu-id="a69d4-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
