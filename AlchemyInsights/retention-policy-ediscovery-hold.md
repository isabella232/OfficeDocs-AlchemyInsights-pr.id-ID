---
title: 2609-retensi-atau-eDiscovery-tahan
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: 85c41995545efd8e1526d9f7dce4a23929f85be5
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994072"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a><span data-ttu-id="f3ff9-102">Tidak dapat menghapus item di SharePoint online atau OneDrive untuk bisnis</span><span class="sxs-lookup"><span data-stu-id="f3ff9-102">Unable to delete items in SharePoint Online or OneDrive for Business</span></span>

<span data-ttu-id="f3ff9-103">Anda atau pengguna Anda mungkin tidak dapat menghapus item di SharePoint online atau OneDrive untuk bisnis karena kebijakan retensi, retensi label atau penahanan eDiscovery diterapkan ke situs SharePoint OneDrive atau item tertentu.</span><span class="sxs-lookup"><span data-stu-id="f3ff9-103">You or your users may be unable to delete items in SharePoint Online or OneDrive for Business because a retention policy, retention label, or eDiscovery hold is applied to a SharePoint of OneDrive site or to a specific item.</span></span> <span data-ttu-id="f3ff9-104">Ini termasuk tidak dapat menghapus dokumen, versi dokumen, folder, pustaka dokumen, daftar, aplikasi, situs, atau koleksi situs.</span><span class="sxs-lookup"><span data-stu-id="f3ff9-104">This includes being unable to delete a document, a document version, a folder, a document library, a list, an app, a site, or a site collection.</span></span> <span data-ttu-id="f3ff9-105">Berikut adalah beberapa contoh dari pesan galat yang mungkin Anda terima jika Anda mencoba untuk menghapus item yang dipertahankan:</span><span class="sxs-lookup"><span data-stu-id="f3ff9-105">Here are some examples of the error messages you may received if you try to delete an item that is being retained:</span></span>

- <span data-ttu-id="f3ff9-106">"Situs ini tidak dapat dihapus karena disertakan dalam kebijakan penyimpanan atau penahanan eDiscovery"</span><span class="sxs-lookup"><span data-stu-id="f3ff9-106">"This site cannot be deleted because it is included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="f3ff9-107">"Situs ini memiliki kebijakan kepatuhan yang ditetapkan untuk memblokir penghapusan"</span><span class="sxs-lookup"><span data-stu-id="f3ff9-107">"This site has a compliance policy set to block deletion"</span></span>
- <span data-ttu-id="f3ff9-108">"Kebijakan kepatuhan saat ini memblokir penghapusan situs ini"</span><span class="sxs-lookup"><span data-stu-id="f3ff9-108">"A compliance policy is currently blocking this site deletion"</span></span>
- <span data-ttu-id="f3ff9-109">"Koleksi situs ini tidak dihapus karena berisi situs yang disertakan dalam kebijakan penyimpanan atau penahanan eDiscovery"</span><span class="sxs-lookup"><span data-stu-id="f3ff9-109">"This site collection can’t be deleted because it contains sites that are included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="f3ff9-110">"Anda harus menghapus semua item dalam folder ini sebelum Anda menghapus folder"</span><span class="sxs-lookup"><span data-stu-id="f3ff9-110">"You have to delete all the items in this folder before you delete the folder"</span></span>
- <span data-ttu-id="f3ff9-111">"Versi item ini tidak dapat dihapus karena kebijakan ditahan atau retensi"</span><span class="sxs-lookup"><span data-stu-id="f3ff9-111">"Versions of this item cannot be deleted because it is on hold or retention policy"</span></span>
- <span data-ttu-id="f3ff9-112">"Item tidak dapat dihapus saat ditahan"</span><span class="sxs-lookup"><span data-stu-id="f3ff9-112">"Item cannot be deleted while on hold"</span></span>
- <span data-ttu-id="f3ff9-113">"Label yang diterapkan untuk item ini mencegah dari sedang diedit atau dihapus"</span><span class="sxs-lookup"><span data-stu-id="f3ff9-113">"The label that's applied to this item prevents it from being edited or deleted"</span></span>
- <span data-ttu-id="f3ff9-114">"Daftar tidak dihapus saat ditahan atau kebijakan retensi"</span><span class="sxs-lookup"><span data-stu-id="f3ff9-114">"List cannot be deleted while on hold or retention policy"</span></span>
- <span data-ttu-id="f3ff9-115">"Daftar tidak dapat dihapus jika diblokir atau kebijakan retensi diterapkan untuk itu"</span><span class="sxs-lookup"><span data-stu-id="f3ff9-115">"The list cannot be deleted if it is blocked or if a retention policy is applied to it"</span></span>

<span data-ttu-id="f3ff9-116">Untuk menghapus item dalam salah satu dari skenario ini, kebijakan retensi, label retensi, atau penahanan eDiscovery harus dihapus (atau situs harus dikecualikan dari kebijakan penyimpanan).</span><span class="sxs-lookup"><span data-stu-id="f3ff9-116">To delete items in one of these scenarios, the retention policy, retention label, or eDiscovery hold has to be removed (or a site has to be excluded from a retention policy).</span></span> <span data-ttu-id="f3ff9-117">Anda perlu menonaktifkan atau mengecualikan masing-masing memegang yang menyebabkan masalah ini.</span><span class="sxs-lookup"><span data-stu-id="f3ff9-117">You need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="f3ff9-118">Setelah kebijakan retensi atau tahan dihapus, mungkin diperlukan waktu hingga 24 jam agar perubahan diterapkan.</span><span class="sxs-lookup"><span data-stu-id="f3ff9-118">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> 

<span data-ttu-id="f3ff9-119">Untuk informasi tentang tentang fitur penyimpanan dan tahan yang berbeda yang dapat diterapkan ke situs SharePoint dan akun OneDrive, lihat salah satu topik berikut.</span><span class="sxs-lookup"><span data-stu-id="f3ff9-119">For information about about the different retention and hold features that can be applied to SharePoint sites and OneDrive accounts, see one of the following topics.</span></span>

- [<span data-ttu-id="f3ff9-120">Ikhtisar kebijakan retensi</span><span class="sxs-lookup"><span data-stu-id="f3ff9-120">Overview of retention policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [<span data-ttu-id="f3ff9-121">Ikhtisar label Penyimpanan</span><span class="sxs-lookup"><span data-stu-id="f3ff9-121">Overview of retention labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [<span data-ttu-id="f3ff9-122">Mengelola pembekuan dalam eDiscovery tingkat lanjut</span><span class="sxs-lookup"><span data-stu-id="f3ff9-122">Manage holds in Advanced eDiscovery</span></span>](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [<span data-ttu-id="f3ff9-123">eDiscovery memegang</span><span class="sxs-lookup"><span data-stu-id="f3ff9-123">eDiscovery holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [<span data-ttu-id="f3ff9-124">Kebijakan penutupan dan penghapusan situs warisan</span><span class="sxs-lookup"><span data-stu-id="f3ff9-124">Legacy site closure and deletion policies</span></span>](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
