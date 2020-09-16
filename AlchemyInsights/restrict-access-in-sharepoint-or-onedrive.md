---
title: Membatasi akses di SharePoint atau OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: d8be1eb5bdcd0b5b08ddad32a45b6282c788c26a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720685"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="a6e16-102">Membatasi akses di SharePoint atau OneDrive</span><span class="sxs-lookup"><span data-stu-id="a6e16-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="a6e16-103">Di SharePoint dan OneDrive, Anda membatasi akses ke item seperti file, folder, dan daftar dengan memberikan akses hanya ke grup atau individu yang ingin Anda akses.</span><span class="sxs-lookup"><span data-stu-id="a6e16-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="a6e16-104">Secara default, izin di SharePoint diwarisi lebih tinggi dalam hierarki.</span><span class="sxs-lookup"><span data-stu-id="a6e16-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="a6e16-105">Jadi file mewarisi izinnya dari folder, yang mewarisi izinnya dari Pustaka, yang mewarisi izinnya dari situs.</span><span class="sxs-lookup"><span data-stu-id="a6e16-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="a6e16-106">Anda bisa berbagi di tingkat yang lebih tinggi (seperti dengan berbagi seluruh situs) lalu memisahkan warisan jika Anda tidak ingin berbagi semua item di situs.</span><span class="sxs-lookup"><span data-stu-id="a6e16-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="a6e16-107">Namun, kami tidak merekomendasikan hal ini karena membuat mempertahankan izin yang lebih kompleks dan membingungkan di masa mendatang.</span><span class="sxs-lookup"><span data-stu-id="a6e16-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="a6e16-108">Berikut yang bisa Anda lakukan sebagai gantinya:</span><span class="sxs-lookup"><span data-stu-id="a6e16-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="a6e16-109">Jika, misalnya, Anda ingin berbagi semua konten folder kecuali satu file di dalamnya, Pindahkan file tersebut ke lokasi baru yang tidak dibagikan.</span><span class="sxs-lookup"><span data-stu-id="a6e16-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="a6e16-110">Jika Anda memiliki dua subfolder dalam folder, dan Anda ingin berbagi satu subfolder dengan grup A dan B dan hanya memperbolehkan mengelompokkan akses ke subfolder kedua, bagikan folder induk dengan grup A dan tambahkan Grup B ke subfolder pertama.</span><span class="sxs-lookup"><span data-stu-id="a6e16-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="a6e16-111">Berhenti berbagi file atau folder </span><span class="sxs-lookup"><span data-stu-id="a6e16-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

