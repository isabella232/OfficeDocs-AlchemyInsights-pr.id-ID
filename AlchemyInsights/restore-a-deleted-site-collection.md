---
title: Memulihkan situs yang dihapus
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 570284765f32212b4ef2062db5b70f427b28c121
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47692046"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="820e6-102">Memulihkan situs yang dihapus</span><span class="sxs-lookup"><span data-stu-id="820e6-102">Restore a deleted site</span></span>

<span data-ttu-id="820e6-103">Saat admin menghapus situs SharePoint, admin ditempatkan di keranjang sampah kumpulan situs, tempat file disimpan selama 93 hari sebelum dihapus secara permanen.</span><span class="sxs-lookup"><span data-stu-id="820e6-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="820e6-104">Untuk memulihkan situs:</span><span class="sxs-lookup"><span data-stu-id="820e6-104">To restore the site:</span></span>
  
1. <span data-ttu-id="820e6-105">Di pusat admin SharePoint baru, klik **keranjang sampah** pada pita.</span><span class="sxs-lookup"><span data-stu-id="820e6-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="820e6-106">Pilih kotak centang di samping kumpulan situs yang ingin Anda Pulihkan.</span><span class="sxs-lookup"><span data-stu-id="820e6-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="820e6-107">Klik **Pulihkan Item terhapus**.</span><span class="sxs-lookup"><span data-stu-id="820e6-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="820e6-108">Untuk memulihkan situs komunikasi yang dihapus, Anda bisa menggunakan pusat admin SharePoint yang baru.</span><span class="sxs-lookup"><span data-stu-id="820e6-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="820e6-109">Jika tidak, Anda perlu menggunakan Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="820e6-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="820e6-110">Untuk memulihkan situs yang termasuk dalam grup Microsoft 365, Anda perlu memulihkan grup di pusat admin Exchange.</span><span class="sxs-lookup"><span data-stu-id="820e6-110">To restore a site that belongs to a Microsoft 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="820e6-111">Grup dapat dipulihkan selama 30 hari setelah dihapus.</span><span class="sxs-lookup"><span data-stu-id="820e6-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

