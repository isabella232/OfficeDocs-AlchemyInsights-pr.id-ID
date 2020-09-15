---
title: Situs modern sebagai situs akar
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666873"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="6bfd1-102">Situs modern sebagai situs akar</span><span class="sxs-lookup"><span data-stu-id="6bfd1-102">Modern site as root site</span></span>

<span data-ttu-id="6bfd1-103">Kami telah mulai meluncurkan fitur baru yang akan memungkinkan Anda untuk [menukar situs root situs klasik Anda dengan situs modern](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="6bfd1-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="6bfd1-104">Gunakan [invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) untuk menukar lokasi situs dengan situs lain saat mengarsipkan situs asli.</span><span class="sxs-lookup"><span data-stu-id="6bfd1-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="6bfd1-105">Tersedia untuk kedua situs tim (tidak tersambung ke grup) dan situs komunikasi.</span><span class="sxs-lookup"><span data-stu-id="6bfd1-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="6bfd1-106">Jangan menghapus situs akar klasik Anda untuk membuat situs komunikasi modern.</span><span class="sxs-lookup"><span data-stu-id="6bfd1-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="6bfd1-107">Ini tidak didukung oleh Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6bfd1-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="6bfd1-108">Menghapus situs akar akan membuat semua situs SharePoint di organisasi Anda tidak dapat diakses oleh semua pengguna, hingga Anda memulihkan situs atau membuat situs baru di URL yang sama.</span><span class="sxs-lookup"><span data-stu-id="6bfd1-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="6bfd1-109">Kami akan mengkomunikasikan fitur ini melalui pusat pesan.</span><span class="sxs-lookup"><span data-stu-id="6bfd1-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="6bfd1-110">Anda akan diminta untuk mengaktifkan fitur dalam penyewa Anda.</span><span class="sxs-lookup"><span data-stu-id="6bfd1-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="6bfd1-111">Masalah yang diketahui dengan situs bertukar</span><span class="sxs-lookup"><span data-stu-id="6bfd1-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="6bfd1-112">Situs target mungkin mengembalikan kesalahan "tidak ditemukan" (HTTP 404) untuk periode waktu yang singkat.</span><span class="sxs-lookup"><span data-stu-id="6bfd1-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="6bfd1-113">Konten harus diberi kembali untuk memperbarui indeks pencarian.</span><span class="sxs-lookup"><span data-stu-id="6bfd1-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="6bfd1-114">Tidak ada langkah manual yang diperlukan di sini, ini akan dilakukan secara otomatis.</span><span class="sxs-lookup"><span data-stu-id="6bfd1-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="6bfd1-115">Apa pun yang bergantung pada tautan "statis" (seperti file sinkronisasi file dan OneNote) perlu dikoreksi secara manual.</span><span class="sxs-lookup"><span data-stu-id="6bfd1-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="6bfd1-116">Situs Project Server mungkin perlu divalidasi untuk memastikan bahwa situs tersebut masih terkait dengan benar.</span><span class="sxs-lookup"><span data-stu-id="6bfd1-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
