---
title: Situs modern sebagai situs akar
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 2e2bb02b9dbaf7f8ede0b4c5ba8c8f29453309cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054705"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="6417a-102">Situs modern sebagai situs akar</span><span class="sxs-lookup"><span data-stu-id="6417a-102">Modern site as root site</span></span>

<span data-ttu-id="6417a-103">Kami telah mulai peluncuran fitur baru yang akan memungkinkan Anda untuk [swap situs akar situs klasik Anda dengan situs modern](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="6417a-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="6417a-104">Gunakan [invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) untuk menukar lokasi situs dengan situs lain saat pengarsipan situs asli.</span><span class="sxs-lookup"><span data-stu-id="6417a-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="6417a-105">Tersedia untuk kedua tim situs (tidak terhubung ke grup) dan situs komunikasi.</span><span class="sxs-lookup"><span data-stu-id="6417a-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="6417a-106">Jangan menghapus situs root klasik Anda untuk membuat situs komunikasi modern.</span><span class="sxs-lookup"><span data-stu-id="6417a-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="6417a-107">Hal ini tidak didukung oleh Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6417a-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="6417a-108">Menghapus situs akar akan membuat semua situs SharePoint di organisasi Anda tidak dapat diakses oleh semua pengguna, sampai Anda memulihkan situs atau membuat situs baru di URL yang sama.</span><span class="sxs-lookup"><span data-stu-id="6417a-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="6417a-109">Kami akan mengkomunikasikan fitur ini melalui pusat pesan.</span><span class="sxs-lookup"><span data-stu-id="6417a-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="6417a-110">Anda harus mengharapkan fitur yang akan diaktifkan di penyewa Anda segera.</span><span class="sxs-lookup"><span data-stu-id="6417a-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="6417a-111">Masalah yang diketahui dengan swapping Sites</span><span class="sxs-lookup"><span data-stu-id="6417a-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="6417a-112">Situs target dapat mengembalikan galat "tidak ditemukan" (HTTP 404) untuk jangka waktu yang singkat.</span><span class="sxs-lookup"><span data-stu-id="6417a-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="6417a-113">Konten harus di-recrawled untuk memperbarui indeks pencarian.</span><span class="sxs-lookup"><span data-stu-id="6417a-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="6417a-114">Tidak ada langkah manual yang diperlukan di sini, ini akan dilakukan secara otomatis.</span><span class="sxs-lookup"><span data-stu-id="6417a-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="6417a-115">Apa pun tergantung pada "statis" link (seperti file Sync dan OneNote file) harus dikoreksi secara manual.</span><span class="sxs-lookup"><span data-stu-id="6417a-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="6417a-116">Proyek server situs mungkin perlu divalidasi untuk memastikan bahwa mereka masih terkait dengan benar.</span><span class="sxs-lookup"><span data-stu-id="6417a-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
