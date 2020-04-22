---
title: Membatasi akses di SharePoint atau OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: ed8e97b20c96a7b46995c969074cc4cef3a787d9
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715887"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="b1b56-102">Membatasi akses di SharePoint atau OneDrive</span><span class="sxs-lookup"><span data-stu-id="b1b56-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="b1b56-103">Di SharePoint dan OneDrive, Anda membatasi akses ke item seperti file, folder, dan daftar dengan memberikan akses hanya ke grup atau individu yang Anda ingin memiliki akses.</span><span class="sxs-lookup"><span data-stu-id="b1b56-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="b1b56-104">Secara default, izin di SharePoint diwariskan dari lebih tinggi dalam hirarki.</span><span class="sxs-lookup"><span data-stu-id="b1b56-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="b1b56-105">Jadi file mewarisi izin dari folder, yang mewarisi izin dari Perpustakaan, yang mewarisi izin dari situs.</span><span class="sxs-lookup"><span data-stu-id="b1b56-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="b1b56-106">Anda dapat berbagi di tingkat yang lebih tinggi (seperti dengan berbagi seluruh situs) dan kemudian Break warisan jika Anda tidak ingin berbagi semua item di situs.</span><span class="sxs-lookup"><span data-stu-id="b1b56-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="b1b56-107">Namun, kami tidak menyarankan ini karena itu membuat menjaga hak akses yang lebih kompleks dan membingungkan di masa depan.</span><span class="sxs-lookup"><span data-stu-id="b1b56-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="b1b56-108">Berikut adalah apa yang bisa Anda lakukan sebagai gantinya:</span><span class="sxs-lookup"><span data-stu-id="b1b56-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="b1b56-109">Jika, misalnya, Anda ingin berbagi semua konten folder kecuali satu berkas di dalamnya, memindahkan berkas tersebut ke lokasi baru yang tidak dibagi.</span><span class="sxs-lookup"><span data-stu-id="b1b56-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="b1b56-110">Jika Anda memiliki dua subfolder di folder, dan Anda ingin berbagi satu subfolder dengan grup A dan B dan mengizinkan hanya grup akses ke subfolder kedua, berbagi folder induk dengan grup A dan menambahkan Grup B ke subfolder pertama.</span><span class="sxs-lookup"><span data-stu-id="b1b56-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="b1b56-111">Berhenti berbagi file atau folder</span><span class="sxs-lookup"><span data-stu-id="b1b56-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

