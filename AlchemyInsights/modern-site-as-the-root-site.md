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
ms.openlocfilehash: 2f75f1e60af06da47fe846e84bbb370dd60084e9
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36543856"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="86b0f-102">Situs modern sebagai situs akar</span><span class="sxs-lookup"><span data-stu-id="86b0f-102">Modern site as root site</span></span>

<span data-ttu-id="86b0f-103">Kami telah mulai untuk peluncuran fitur baru yang akan memungkinkan Anda untuk menukar situs akar klasik situs Anda dengan situs modern.</span><span class="sxs-lookup"><span data-stu-id="86b0f-103">We have begun to rollout a new feature that will allow you to swap your classic site root site with a modern site.</span></span> <span data-ttu-id="86b0f-104">Gunakan [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) untuk menukar lokasi situs dengan situs lain sementara pengarsipan situs asli.</span><span class="sxs-lookup"><span data-stu-id="86b0f-104">Use [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="86b0f-105">Tersedia untuk tim situs (tidak terhubung ke grup) dan komunikasi situs.</span><span class="sxs-lookup"><span data-stu-id="86b0f-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

>[!Important]
> <span data-ttu-id="86b0f-106">Tidak menghapus situs akar klasik untuk membuat situs komunikasi modern.</span><span class="sxs-lookup"><span data-stu-id="86b0f-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="86b0f-107">Hal ini tidak didukung oleh Microsoft.</span><span class="sxs-lookup"><span data-stu-id="86b0f-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="86b0f-108">Menghapus situs akar akan membuat semua situs SharePoint dalam organisasi Anda tidak dapat diakses untuk semua pengguna, sampai Anda mengembalikan situs atau membuat situs baru di URL yang sama.</span><span class="sxs-lookup"><span data-stu-id="86b0f-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="86b0f-109">Kita akan berkomunikasi melalui pusat pesan fitur ini.</span><span class="sxs-lookup"><span data-stu-id="86b0f-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="86b0f-110">Anda harus mengharapkan fitur harus diaktifkan di penyewa Anda segera.</span><span class="sxs-lookup"><span data-stu-id="86b0f-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="86b0f-111">Masalah yang dikenal dengan menukar situs</span><span class="sxs-lookup"><span data-stu-id="86b0f-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="86b0f-112">Situs target mungkin kembali "tidak ditemukan" kesalahan (HTTP 404) untuk periode waktu yang singkat.</span><span class="sxs-lookup"><span data-stu-id="86b0f-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="86b0f-113">Konten akan perlu recrawled untuk memperbarui indeks pencarian.</span><span class="sxs-lookup"><span data-stu-id="86b0f-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="86b0f-114">Tidak ada langkah manual yang diperlukan di sini, ini akan dilakukan secara otomatis.</span><span class="sxs-lookup"><span data-stu-id="86b0f-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="86b0f-115">Apa pun yang bergantung pada "statis" link (seperti File Sync dan OneNote file) akan perlu diperbaiki secara manual.</span><span class="sxs-lookup"><span data-stu-id="86b0f-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="86b0f-116">Lokasi Server proyek mungkin perlu divalidasi untuk memastikan bahwa mereka masih berhubungan dengan benar.</span><span class="sxs-lookup"><span data-stu-id="86b0f-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
