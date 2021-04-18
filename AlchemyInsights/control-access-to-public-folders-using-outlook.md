---
title: Kontrol akses ke folder publik menggunakan Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816743"
---
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="ac68c-102">Kontrol akses ke folder publik menggunakan Outlook</span><span class="sxs-lookup"><span data-stu-id="ac68c-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="ac68c-103">Untuk mengontrol pengguna mana yang dapat mengakses folder publik menggunakan Outlook:</span><span class="sxs-lookup"><span data-stu-id="ac68c-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="ac68c-104">Gunakan `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span><span class="sxs-lookup"><span data-stu-id="ac68c-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="ac68c-105">$true: Izinkan pengguna mengakses folder publik di Outlook</span><span class="sxs-lookup"><span data-stu-id="ac68c-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="ac68c-106">$false: Cegah pengguna mengakses folder publik di Outlook.</span><span class="sxs-lookup"><span data-stu-id="ac68c-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="ac68c-107">Ini adalah nilai default.</span><span class="sxs-lookup"><span data-stu-id="ac68c-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="ac68c-108">Catatan: Prosedur ini hanya dapat mengontrol koneksi dengan Outlook versi desktop untuk klien Windows.</span><span class="sxs-lookup"><span data-stu-id="ac68c-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="ac68c-109">Pengguna dapat terus mengakses folder publik menggunakan OWA atau Outlook untuk Mac.</span><span class="sxs-lookup"><span data-stu-id="ac68c-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="ac68c-110">Untuk informasi selengkapnya, lihat [Koneksi Terkontrol ke Folder Publik di Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="ac68c-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
