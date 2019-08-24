---
title: Situs modern sebagai situs akar
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: d5ea73c967013822854dbd408d4628d991c90378
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620762"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="c243d-102">Situs modern sebagai situs akar</span><span class="sxs-lookup"><span data-stu-id="c243d-102">Modern site as root site</span></span>

<span data-ttu-id="c243d-103">Kami telah mulai untuk peluncuran fitur baru yang akan memungkinkan Anda untuk menukar situs akar klasik situs Anda dengan situs modern.</span><span class="sxs-lookup"><span data-stu-id="c243d-103">We have begun to rollout a new feature that will allow you to swap your classic site root site with a modern site.</span></span> <span data-ttu-id="c243d-104">Gunakan [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) untuk menukar lokasi situs dengan situs lain sementara pengarsipan situs asli.</span><span class="sxs-lookup"><span data-stu-id="c243d-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="c243d-105">Tersedia untuk tim situs (tidak terhubung ke grup) dan komunikasi situs.</span><span class="sxs-lookup"><span data-stu-id="c243d-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

>[!Important]
> <span data-ttu-id="c243d-106">Tidak menghapus situs akar klasik untuk membuat situs komunikasi modern.</span><span class="sxs-lookup"><span data-stu-id="c243d-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="c243d-107">Hal ini tidak didukung oleh Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c243d-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="c243d-108">Menghapus situs akar akan membuat semua situs SharePoint dalam organisasi Anda tidak dapat diakses untuk semua pengguna, sampai Anda mengembalikan situs atau membuat situs baru di URL yang sama.</span><span class="sxs-lookup"><span data-stu-id="c243d-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="c243d-109">Kita akan berkomunikasi melalui pusat pesan fitur ini.</span><span class="sxs-lookup"><span data-stu-id="c243d-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="c243d-110">Anda harus mengharapkan fitur harus diaktifkan di penyewa Anda segera.</span><span class="sxs-lookup"><span data-stu-id="c243d-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="c243d-111">Masalah yang dikenal dengan menukar situs</span><span class="sxs-lookup"><span data-stu-id="c243d-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="c243d-112">Situs target mungkin kembali "tidak ditemukan" kesalahan (HTTP 404) untuk periode waktu yang singkat.</span><span class="sxs-lookup"><span data-stu-id="c243d-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="c243d-113">Konten akan perlu recrawled untuk memperbarui indeks pencarian.</span><span class="sxs-lookup"><span data-stu-id="c243d-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="c243d-114">Tidak ada langkah manual yang diperlukan di sini, ini akan dilakukan secara otomatis.</span><span class="sxs-lookup"><span data-stu-id="c243d-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="c243d-115">Apa pun yang bergantung pada "statis" link (seperti File Sync dan OneNote file) akan perlu diperbaiki secara manual.</span><span class="sxs-lookup"><span data-stu-id="c243d-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="c243d-116">Lokasi Server proyek mungkin perlu divalidasi untuk memastikan bahwa mereka masih berhubungan dengan benar.</span><span class="sxs-lookup"><span data-stu-id="c243d-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
