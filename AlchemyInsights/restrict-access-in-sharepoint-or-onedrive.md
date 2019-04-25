---
title: Membatasi akses dalam SharePoint atau OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e0fbec6eb269a173664e2b9a1efe6eefb527b96f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/23/2019
ms.locfileid: "32383874"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="a423b-102">Membatasi akses dalam SharePoint atau OneDrive</span><span class="sxs-lookup"><span data-stu-id="a423b-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="a423b-103">SharePoint dan OneDrive, Anda membatasi akses ke barang-barang seperti file, folder, dan daftar dengan memberikan akses hanya untuk kelompok atau individu yang ingin memiliki akses.</span><span class="sxs-lookup"><span data-stu-id="a423b-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="a423b-104">Secara default, izin di SharePoint diwariskan dari up lebih tinggi dalam hirarki.</span><span class="sxs-lookup"><span data-stu-id="a423b-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="a423b-105">Jadi file mewarisi dengan izin dari folder, yang mewarisi dengan izin dari Perpustakaan, yang mewarisi dengan izin dari situs.</span><span class="sxs-lookup"><span data-stu-id="a423b-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="a423b-106">Anda dapat berbagi di tingkat yang lebih tinggi (seperti dengan berbagi seluruh situs) dan istirahat warisan jika Anda tidak ingin untuk berbagi semua item di situs.</span><span class="sxs-lookup"><span data-stu-id="a423b-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="a423b-107">Namun, kami tidak merekomendasikan ini karena membuat mempertahankan izin yang lebih kompleks dan membingungkan di masa depan.</span><span class="sxs-lookup"><span data-stu-id="a423b-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="a423b-108">Berikut adalah apa yang dapat Anda lakukan sebagai gantinya:</span><span class="sxs-lookup"><span data-stu-id="a423b-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="a423b-109">Jika, misalnya, Anda ingin berbagi semua isi folder kecuali satu file di dalamnya, memindahkan file ke lokasi baru yang tidak berbagi.</span><span class="sxs-lookup"><span data-stu-id="a423b-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="a423b-110">Jika Anda memiliki dua subfolder dalam folder, dan Anda ingin berbagi satu subfolder dengan kelompok A dan B dan memungkinkan hanya grup A akses ke subfolder kedua, berbagi folder induk dengan grup A dan menambahkan Grup B ke subfolder pertama.</span><span class="sxs-lookup"><span data-stu-id="a423b-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="a423b-111">Berhenti berbagi file atau folder</span><span class="sxs-lookup"><span data-stu-id="a423b-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

